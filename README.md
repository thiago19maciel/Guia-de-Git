# Guia-de-Git
Neste repositório irei explicar alguns conceitos de Git

## O que é o Git?
O Git é uma ferramenta que auxilia uma equipe de desenvolvedores de software a controlar a versão de um determinado programa.

Para isso, o Git possui um histórico de atualizações, de forma que cada alteração feita por um desenvolvedor, é
salva com data da alteração, o autor, que é a pessoa que fez a alteração, e as mudanças feitas.

O Git faz o controle de versão local, ou seja, apenas na sua máquina. Para salvar na nuvem (remotamente) você pode usar a plataforma Github. 

Para se usar o Git, deve ser feita a instalação dele por meio deste [link](https://git-scm.com/download/win).

Após a instalação do Git, você poderá usar o terminal Git Bash, que é a ferramenta em que serão escritos os comandos.
Agora você deverá abrir o aplicativo Git Bash. <br>

## Vamos configurar seu Git? Não se preocupe, é super fácil
Dica: onde houver o simbolo <> voce deve digitar o que desejar. <br>
Siga as instruções:
- Configurando seu nome de usuário, digite o comando
```
  git config --global user.name <nome>
```

- Semelhante ao nome, para configurar seu e-mail, digite o comando
```
  git config --global user.email <email>
```

Viu como é fácil? Git configurado, bora aprender a usar seus principais comandos :)

## Criando um repositório local
Dica: onde houver o simbolo <> voce deve digitar o nome que desesjar. <br>

No Git bash você devera utilizar os seguintes comandos:

- Para criar um repositório local, ou seja, a pasta que você irá usar em seu computador, digite o comando:
```
  mkdir <nome-do-repositorio>
```

- Com o repositório local criado, agora iremos entrar no repositorio, digite o comando:
```
  cd <nome-do-repositorio>
```

- Agora que estamos dentro do repositório, devemos adicionar o controle de versão Git ao repositorio, digite o comando:
```
  git init
```
  
## Subindo um repositório local para o repositório remoto (Github)
Para fazer isso, primeiro você deve criar entrar com seu login no Github. Caso não tenha login, pode clicar [aqui](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) para fazer seu login.

Feito o Login, você deve criar um novo repositório. Para isso, clique no + no canto direito em cima da tela, e novo repositório.
Dê um nome para esse repositório, selecione a opção de adicionar um README.md, que é uma descrição do projeto.
Confirme a criação do repositório.
  
Criado o novo repositorio, vamos conectar o nosso repo local, que é a pasta do projeto.
- Para fazer isso, clique no botão verde escrito code, selecione e copie o link.
 
- Abra o Git bash, e digite o comando colando o link:
```
  git remote add origin <link>
```
  
Agora você já conectou o repo local com o repositório remoto, ou seja, o Github.

## Colocando seus códigos no repositório local
Dica: onde houver o simbolo <> voce deve digitar o que desesjar. <br>
Conforme voce for fazendo seus códigos, você deve mostrar ao Git que eles existem e devem ser ADICIONADOS ao repositório.
- Para adicionar os arquivos, digite o comando:
```
  git add *
```

Arquivos adicionados, agora devemos fazer o commit, que é dizer ao Git que o arquivo está pronto.
- Para fazer o commit (ou commitar), digite o comando:
```
  git commit -m "<mensagem>"
```
A parte <mensagem> serve para descrever o que foi feito naquele momento, por exemplo: adicionar botão de login, validação de usuário.
  
Agora você já tem seu repositório local criado, vamos subir ele para o Github, que é uma forma de disponibilizar o nosso código para o mundo.
  
- Para subir seus códigos do repositório local para o Github, digite o comando:
```
  git push origin master
```
  
# Pronto :). Agora você já sabe usar o Git e o Github
