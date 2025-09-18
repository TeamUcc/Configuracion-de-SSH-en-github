# Configuracion-de-SSH-en-github

## 1) Generación de una nueva clave SSH y adición al agente SSH
``
https://docs.github.com/es/enterprise-cloud@latest/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
``
Puedes generar una nueva clave SSH en el equipo local. Después de generar la clave, puede agregar la clave pública a la cuenta en GitHub.com para habilitar la autenticación para las operaciones de Git a través de SSH.



## Abra Terminal.
## 2) Pega el texto siguiente, reemplazando el correo electrónico usado en el ejemplo por tu dirección de correo electrónico de GitHub.
 ``
 ssh-keygen -t ed25519 -C "your_email@example.com"
 ``

Esto crea una llave SSH utilizando el correo electrónico proporcionado como etiqueta.

> Generating public/private ALGORITHM key pair.


Cuando se te pida: "Introduce un archivo en el que se pueda guardar la clave", teclea Enter para aceptar la ubicación de archivo predeterminada. Ten en cuenta que si ya creaste claves SSH anteriormente, ssh-keygen puede pedirte que vuelvas a escribir otra clave. En este caso, se recomienda crear una clave SSH con nombre personalizado. Para ello, escribe la ubicación de archivo predeterminada y reemplaza id_ALGORITHM por el nombre de clave personalizado.

> Enter a file in which to save the key (/home/YOU/.ssh/id_ALGORITHM):[Press enter]
> Enter passphrase (empty for no passphrase): [Type a passphrase]

##  3) Cuando se le pida, escriba una frase de contraseña segura. Para más información, consulta 
> Enter same passphrase again: [Type passphrase again]



## Agregar una clave SSH nueva a tu cuenta de GitHub
Copia la llave SSH pública a tu portapapeles.

Si tu archivo de llave SSH pública tiene un nombre diferente que en el código de ejemplo, modifica el nombre de archivo para que coincida con tu configuración actual. Al copiar tu clave, no agregues líneas nuevas o espacios en blanco.

``
 cat ~/.ssh/id_ed25519.pub
``


## Crea una nueva SSH key 
<img width="928" height="132" alt="image" src="https://github.com/user-attachments/assets/25fa3c51-aaa5-4d85-bb82-e7ad878fa930" />

##  ya puedes clonar el repo
<img width="429" height="318" alt="image" src="https://github.com/user-attachments/assets/52e431ea-c739-46cb-b703-5bdd084c2251" />

 
