# instrucciones_git
Guía para creación, carga y descarga de fuentes a repositorios

** Parametro para paths largos
git config --global core.longpaths true

**MAQUINA ORIGEN 
--(Cargar los archivos al repositorio)
git init
git add .  
git commit -m "comentarios"
git branch -M master 
git remote add origin https://github.com/JrgDz/graphql.git (HTTPS)
git push -u origin master

**MAQUINA DESTINO 
--(Gitbash)
ssh-keygen -t rsa -b 4096 -C "1710.j.diaz.sanchez@gmail.com"
eval $(ssh-agent -s)
ssh-add ~/.ssh/id_rsa
cat ~/.ssh/id_rsa.pub

**EXPLORADOR WEB 
--(Github.com)
Crear la key ssh

**MAQUINA DESTINO 
--(Descargar los archivos del repositorio) 
Crear carpeta y abrir terminal
git init
git remote add origin git@github.com:JrgDz/graphql.git (SSH)
git pull origin master (password: veneno86)
git status
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
--(Cargar los archivos al repositorio)
git add .
git commit -m "comentarios"
git status
git push origin master

**MAQUINA ORIGEN 
--(Descargar los archivos del repositorio)
git fetch origin
git merge origin/master
