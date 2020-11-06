# Tutorial de como criar um projeto Django 

### 1. Instale o Python em sua máquina
- Python para Windows - [Baixar](https://www.python.org/downloads/windows/)
- Python para Linux - [Baixar](https://www.python.org/downloads/source/)
  
### 2. Crie um diretório na área de trabalho

- Windows: 
    > cd Desktop

    > md django

- Linux:
    > $ cd Desktop

    > $ mkdir django

### 3. Acesse o [diretrório criando anteriormente](#2-crie-um-diretório-na-área-de-trabalho) e crie uma máquina virtual

- Windows e Linux:
    > cd django

    > py -m venv myvenv


### 4. Instale ou atualize o pip
- Windows e Linux:
    > py -m pip install --upgrade pip

### 5. Inicie a máquina virtual
- Windows e Linux:
    > cd myvenv/Scripts

    > activate

    > No prompt ficará um caminho parecido com esse:     (myvenv) C:\Users\username\Desktop\django\myvenv\Scripts>

- Linux:
    > $ cd myvenv/Scripts

    > $ source activate

    > No bash ficará um caminho parecido com esse:     (myvenv) danilo@Danilo MINGW32 ~/desktop/django/myvenv/scripts

### 6. Instale o Django
- Windows e Linux:
    > pip install Django~=3.0.6

    > Pode ser que demore um pouco.



### 7. Criando e acessando o projeto
- Windows e Linux:
    > django-admin startproject todolist
    ~~~
    De início iremos criar uma lista de tarefas.
    ~~~
    > cd todolist

### 8. Criando base de dados
- Windows e Linux:
    > py manage.py migrate

### 9. Criando o seu usuário adiminstrador
- Windows:
    > py manage.py createsuperuser
- Linux:
    > winpty py manage.py createsuperuser
    ~~~
    OBESERVAÇÃO: 
    Ao preencher os dados do usuário a senha não aparecrá.
    ~~~


### 10. Vamos iniciar a nossa aplicação localmente. Primeiro teste.
- Windows: 
    > py manage.py runserver

    > http://127.0.0.1:8000/
- Linux:
    > winpty py manage.py runserver

    > http://127.0.0.1:8000/

![Navegador](https://tutorial.djangogirls.org/pt/django_start_project/images/install_worked.png)

~~~
    Para cancelar a execução local basta aperatar CTRL + C ou CTRL + BREAK
~~~

### 11. Acessando o Django Admin
- Link: http://127.0.0.1:8000/admin

~~~ 
Tela de login do Django Admin
~~~

![Django Admin](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQNUeS5ybD6rkcsr-_tOJBKLgQwViQ9s63wAg&usqp=CAU)



~~~ 
Tela de home do Django Admin
~~~

![Django Admin](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSLzk_FnbcM6xP9OcsXetmFgmEOo72LlSO1dg&usqp=CAU)


