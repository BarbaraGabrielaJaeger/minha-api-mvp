# Minha API - BARBARA GABRIELA JAEGER
# Sprint: Desenvolvimento Full Stack Básico (40530010058_20240_04)
# Link da API (Swagger): http://172.29.155.70:5000/openapi/swagger#/Produto/add_produto_produto_post

Este pequeno projeto faz parte do material didático da Disciplina **Desenvolvimento Full Stack Básico** 
Com o objetivo de criar uma API , permitir inserir, consultar e excluir dados com Backend em Python.
API documentada com Swagger.
Disciplinas da especialização online **Pós-Graduação em Desenvolvimento Full Stack**, do Departamento de Informática da PUC-Rio.

Códigos das disciplinas da especialização online **Pós-Graduação em Desenvolvimento Full Stack**, do Departamento de Informática da PUC-Rio.

Coordenação: **Prof. Marcos Kalinowski** (*kalinowski@inf.puc-rio.br*)
Professores: Marisa e Angelo
Aluna: Barbara Gabriela Jaeger

# Requisitos :
    # Tecnologias utilizadas: conforme indicado nas aulas.
    # Funcionalidades implementadas:
    # Criar uma API.
    # Inserir, deletar e consultar dados.
    # Backend em Python.
    # Frontend em HTML.
    # URL de acesso ao banco de dados sqlite local (__init__.py).
    # API documentada com Swagger.
    # Interface Frontend adequada, conforme contrato de comunicação e métodos.
    # Backend e Frontend alinhados.
    
##  Registro dos comandos basicos
1. Ambiente de Desenvolvimento (Linux)
Usar terminal WSL (Windows Subsystem for Linux) para criar o ambiente de desenvolvimento:

Instalar WSL
No terminal WSL, siga os seguintes passos
   Dica dos professores
   Vantagem: Criar o ambiente terminal, e não na maquina local
   https://learn.microsoft.com/en-us/windows/wsl/install

2. Instalar python
    sudo apt update
    sudo apt install python3
    -- ver a versão
    python3 --version
    wsl ->   3.12.3
    bash / pws- 3.11.9

    b) Criar e ativar ambiente virtual:
    python3 -m venv venv_api
    source venv_api/bin/activate
   
   c) Instalar pacotes necessários:
   pip install -r requirements.txt

   d) Para desativar o ambiente virtual:
   deactivate

   e) Para reativar o ambiente:
   source venv_api/bin/activate

2. Instalação das Dependências
Caso tenha problemas na instalação de dependências, remova as versões específicas no arquivo requirements.txt e instale novamente:
Flask==2.1.3
Flask-Cors==3.0.10
flask-openapi3==2.1.0
Flask-SQLAlchemy==2.5.1
nose2==0.12.0
pydantic==1.10.2
SQLAlchemy==1.4.41
SQLAlchemy-Utils==0.38.3
typing_extensions==4.3.0
werkzeug==2.0.3

Como Executar
Após clonar o repositório, é necessário estar no diretório raiz do projeto para executar os comandos abaixo.

    a) Instalar dependências:
    É recomendado utilizar um ambiente virtual para instalar as dependências listadas no arquivo requirements.txt:
    (env) $ pip install -r requirements.txt

    b) Executar a API:
    Para iniciar a API, use o comando abaixo:
        bash
        Copiar código
        (env) $ flask run --host 0.0.0.0 --port 5000
        Em modo de desenvolvimento, é recomendado usar o parâmetro --reload, que reiniciará automaticamente o servidor após mudanças no código-fonte:

        bash
        Copiar código
        (env) $ flask run --host 0.0.0.0 --port 5000 --reload

     c) Acessar a API:
      Abra o Swagger UI no navegador para verificar o status da API em execução.

    Para Parar o Servidor:
    Pressione CTRL + C no terminal.

Mais Informações
Este projeto faz parte do material didático da Pós-Graduação em Desenvolvimento Full Stack da PUC-Rio, coordenado pelo Prof. Marcos Kalinowski.

Para mais detalhes sobre o curso, acesse:
Desenvolvimento Full Stack - PUC-Rio

Autor: Barbara Gabriela Jaeger
Data: 15/12/2024 versão do projeto v5.0

Alterações Feitas:
    Melhoria na estrutura de títulos e seções.
    Correção ortográfica e gramatical de alguns trechos.
    Melhor organização dos passos de instalação e execução.
    Formatação e padronização do uso do Markdown para facilitar a leitura.
    Essa versão do README está mais clara, organizada e com um foco em facilitar a execução do projeto.

Texto original abaixo
(env)$ pip install -r requirements.txt
```

Este comando instala as dependências/bibliotecas, descritas no arquivo `requirements.txt`.

Para executar a API  basta executar:

```
(env)$ flask run --host 0.0.0.0 --port 5000
```

Em modo de desenvolvimento é recomendado executar utilizando o parâmetro reload, que reiniciará o servidor
automaticamente após uma mudança no código fonte. 
```
(env)$ flask run --host 0.0.0.0 --port 5000 --reload
http://172.29.155.70:5000 -reload
para parar Press CTRL+c
pip install gunicorn
gunicorn -w 4 -b 0.0.0.0:5000 nome_do_seu_arquivo:app
gunicorn -w 4 -b 0.0.0.0:5000 vmeu_app_api:app


Abra o [http://localhost:5000/#/](http://localhost:5000/#/) no navegador para verificar o status da API em execução.

(env)$ flask run --host 0.0.0.0 --port 5000 --reload
```

Abra o [http://localhost:5000/#/](http://localhost:5000/#/) no navegador para verificar o status da API em execução.
