# Guia Básico de Git e GitHub

Esse é um desafio do bootcamp da Digital Innovation One.

## Instalando o Git

[Downloads](https://git-scm.com/downloads)

## Criando um repositório no GitHub

- Dentro da sua conta no GitHub, acesse seus repositórios;
- Clique em <b>New</b> para criar um novo repositório; <br />
    Aqui você poderá dar um nome, adicionar uma descrição e indicar se o repositório será público ou privado:

    <img src="/create-new-repository.png">
    
- Na seção <b>"Initialize this repository with",</b> você poderá adicionar um arquivo README na criação do seu repositório e dentro desse arquivo detalhar o que foi feito no projeto, falar sobre sua utilidade e informar como ele pode ser usado. 
- Também tem a opção para adicionar o arquivo <b>.gitignore</b> que diz ao Git quais arquivos ou pastas ele deve ignorar em um projeto. 
- Para finalizar, tem a opção de <b>escolher uma licença</b> para que seu repositório seja considerado como código aberto e outros desenvolvedores tenham a liberdade de usar, alterar e distribuir. <br />
    Após isso, você clica em <b>Create repository</b> e pronto, seu repositório remoto estará criado :tada:
    
    <img src="/repository-settings.png">    

- Após criado o repositório no GitHub, vai aparecer alguns comandos que você utilizará para configurar seu repositório local e fazer a conexão entre o repositório local e o remoto. 

    <img src="/command-line-git.png">

## Criando um repositório local

- Crie uma pasta no seu computador
- Abra esta pasta no VSCode e crie um arquivo, pode ser um README.md 
- Voltando para a pasta, abra o Git Bash que foi instalado anteriormente clicando com o botão direito do mouse e depois clicando em <b>Git Bash Here</b>
- Dentro do terminal do Git, digite `git init` para inicializar seu repositório
- Adicione o arquivo que está dentro da pasta com o comando `git add README.md ` ou se tiver mais de um arquivo, pode usar `git add .` que vai adicionar todos os arquivos 
- Depois faça o commit utilizando o comando `git commit -m "nome do commit"`
- Para mudar o nome da branch, utilize o comando `git branch -M main`
- Agora para conectar o repositório local com o repositório criado no GitHub, use o comando `git remote add origin <link do repositório>`
- Agora para empurrar o repositório local para o GitHub, utilize o comando `git push -u origin main`
  
  :tada: Seu reporitório local e o remoto estão conectados :tada: 