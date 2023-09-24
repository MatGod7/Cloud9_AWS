# Cloud9_AWS
This is a repository about cloud9 in AWS

En este readme se guardarán los comandos para hacer un buen repositorio y que significa cada comando.

Primero se debe conectar con el repositorio de github mediante la consola, para ello se utiliza el comando:

ssh-keygen -t rsa , junto con un "enter" se genera una public key. En este caso se llama "/home/ec2-user/.ssh/id_rsa.pub"

por tanto se copia esa llave y se utiliza el comando cat junto con la llave de la siguiente forma "cat /home/ec2-user/.ssh/id_rsa.pub"

Esa llave generada (que son un monton de letras y nuemeros juntos) se copia y se pega en el github, en la seccion: settings/SSH and GPG keys

Se crea una nueva key "new SSH key" y se pega la key generada. Ahora si se puede conectar con el repositorio con el comando: git clone y el link que da github en Code/ SSH


Una vez clonado el repositorio se entra en él con "cd nombre-del-repo" y se crean las cuatro cosas principales: 

Makefile, 
hello.py (el codigo python),
test_hello.py(el codigo para probar el principal),
requirements.txt (basicamente un texo que dice los requerimientos para correr el código)

Y por ultimo crear un entorno virtual de python (es una buena práctica) con " git remote -v" y luego python3 -m venv ~/.nombre-entorno-virtual (buena practica es llamarlo igual que el repo)

Luego un "source ~/.nombre-entorno-virtual/bin/activate" esto activa el entorno virtual

Para verificar que uno esta dentro del entorno se usa " which python"



En el Makefile se utilizan varios comandos para actualizar y probar cosas. (ver comentarios de Makefile para más detalles)



Para saber algunas de las cosas en las que esta fallando el código de manera interactiva, se utlizan los Github actions.

[![Python application test with Github Actions](https://github.com/MatGod7/Cloud9_AWS/actions/workflows/main.yml/badge.svg)](https://github.com/MatGod7/Cloud9_AWS/actions/workflows/main.yml)

