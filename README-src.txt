1)  Poner todos los archivos del codigo en la carpeta SRC

3)  necesito ejecutar el index.py
    desde Scripts>python ..\..\src\index.py




4)  heroku para subirlo
    python web>heroku login

    requirements.txt en \src
    desde scripts> pip freeze > ..\..\src\
    runtime.txt en \src
    desde scripts>python --version 
        python-3.9.0
    Procfile en \src
        web: gunicorn index:app

5)  dentro de src crear repositor de git
    desde src>git init
    src>git add .
    src>git commit -m "subida app"

6)  crear app de heroku desde src>
    heroku create NOMBRE (sino vacio y crea nombre aleatorio)

7)  enlazar la direccion con el proyecto
    src>heroku git:remote NOMBRE

se ha establecido como repositorio remoto a heroku

8) src>git push heroku master

9) >heroku open  o con la direccion