# usando-git-exemplo

Um projeto simples de teste do Git e Github.

## Variável de Ambiente

```flask
python -m venv venv
venv\Scripts\activate
```

## Install

```flask
pip install - requirements.txt

pip install Flask
```

## Run

```flask
$env:FLASK_APP="main.py"
$env:FLASK_ENV=development
flask run
```

## Libs com dependências

```flask
clear
pip freeze
pip freeze > requirements.txt
```

criando o arquivo de libs com as dependências, apagar as outras dependências, deixar apenas o Flask.

## Inicializar o Git

```git
git init
```

## Demais comandos Git

criando o arquivo .gitignore usando touch ou manualmente

```flask
touch .gitignore
```

dizemos ao git os arquivos que não vamos subir para o repositório

```flask

      venv
      __pycache__
      %.pyc
```

colocando em stage todos os arquivos que eu quero subir para o github

```flask
git init
clear
git status
git add -A
```

* garantindo que a branch que estamos usando é a Main
* conectando o meu git ao repositório que eu criei no github
* fazendo o primeiro push do seu commit no seu repositório

```flask
git status
git commit -m "first commit"
git status

git branch -M main 

git remote add origin git@github.com:hibernon/usando-git-exemplo.git

git push -u origin main
```

atualizando a a página do seu repositório (através da tecla F5)

## Fazer modificação após primeiro commit

modifica o código ou um arquivo (README, por exemplo: dar um run)

```flask
git status (para ver quais arquivos foram modificados)
clear
git add -A
git commit -m "alterando retorno da api do Flask e o arquivo README"
clear
git push origin main (enviar o commit para o repositório)
```
