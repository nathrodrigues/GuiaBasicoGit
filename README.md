# Guia Básico de Git e GitHub

Esse é um desafio do bootcamp da Digital Innovation One.

## Instalando o Git

[Downloads](https://git-scm.com/downloads)

## Criando um repositório no GitHub

- Dentro da sua conta no GitHub, acesse seus repositórios
- Clique em <b>New</b> para criar um novo repositório <br />
    Aqui você poderá dar um nome, adicionar uma descrição e indicar se o repositório será público ou privado: <br>

    <img src="/img/create-new-repository.png"> <br />
    
- Na seção <b>"Initialize this repository with",</b> você poderá adicionar um arquivo README na criação do seu repositório e dentro desse arquivo detalhar o que foi feito no projeto, falar sobre sua utilidade e informar como ele pode ser usado
- Também tem a opção para adicionar o arquivo <b>.gitignore</b> que diz ao Git quais arquivos ou pastas ele deve ignorar em um projeto
- Para finalizar, tem a opção de <b>escolher uma licença</b> para que seu repositório seja considerado como código aberto e outros desenvolvedores tenham a liberdade de usar, alterar e distribuir <br />
    Após isso, você clica em <b>Create repository</b> e pronto, seu repositório remoto estará criado :tada: <br>
    
    <img src="/img/repository-settings.png"><br />

- Após criado o repositório no GitHub, vai aparecer alguns comandos que você utilizará para configurar seu repositório local e fazer a conexão entre o repositório local e o remoto <br />

    <img src="/img/command-line-git.png">

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

## Clonando um repositório

- Se você quiser baixar algum repositório basta entrar nele, clicar em <b>Code</b> 
- Vai aparecer um link que você pode copiar <br />    
  
    <img src="/img/clone.png"> <br />

- No terminal do git (ou no terminal no VSCode), você usa o comando `git clone <link copiado do repositório>` e o repositório será baixado no seu computador

## Fazendo Fork de um repositório

- Se você quiser trazer o repositório de alguém para o seu no GitHub, entre no repositório que você quer puxar e clique no botão que está escrito <b>Fork</b>.

## Branch 

- Branches são ramificações dentro do projeto, se você está fazendo um projeto em grupo, poderá criar uma branch para adicionar seu código ou fazer alterações no código principal e depois que ele for revisado, é possível fazer um `merge` da sua branch com a main. <br />

    <img src="/img/git-branches-merge.png"> <br />

- Para criar uma nova branch, use o comando `git checkout -b "nome da branch"`, agora você vai estar dentro da sua nova branch e pode escrever seu código ou fazer alterações no código principal
- Se você quiser trocar de branch use o comando `git checkout nome-da-branch`, por exemplo, voltando para a main `git checkout main`

## Merge 

- Para juntar a sua branch com a branch principal (nesse caso a main), entre na main e digite o código `git merge nome-da-sua-branch` e agora as alterações da sua branch estão na main

## Pull 

- Quando você fizer alterações no seu repositório do GitHub ou fizer <b>clone</b> de algum repositório e depois o autor fizer alterações, basta usar o comando `git pull` para puxar as alterações realizadas no GitHub para sua máquina  

## Pull request 

- Pull requests permite que você informe a outras pessoas sobre as alteraçõesque você fez push para uma branch em um repositório no GitHub. Depois que uma pull request é aberta, você pode discutir e revisar as possíveis alterações com colaboradores e adicionar commits de acompanhamento antes que as alterações sofram merge no branch base.
- Você pode ir em `Pull requests` e para adicionar clique em `New pull request`

## Links úteis 

[Documentação Git](https://git-scm.com/doc)
[Documentação GitHub](https://docs.github.com/pt)