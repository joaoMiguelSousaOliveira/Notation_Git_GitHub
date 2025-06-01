# GIT

### 1. Chegar na pasta do projeto
Utilize de cd no terminal para chegar na pasta do projeto

### 2. Git Init
**`Digite git init para iniciar o Git`**
```Git
git init
```   

### 3. Git Status
**`Retorna o status atual do repositório:`** Quantos branchs, commits e arquivos que ainda não estão no repositório existem.

```Git
git status
```  

### 4. Git add
**`Adiciona os arquivos na área de Stage`**

**`Para adicionar todos arquivos no Stage`**
```Git
git add .
```    
**`Para adicionar um arquvi especifíco no Stage`**
```Git
git nome_do_arquivo.html
```    

### 5. Configurar o Usuário

**`Defina o seu nome de usuário`**
```Git
git config --global user.name seu_nome
```    

**`Defina o seu email`**

```Git
git config --global user.email seu_email
```    

### 6. Git Commit 
**`Para mandar os arquivos do Stage para o repositório Git`**

```Git
git commit -m "mensagem_descritiva_da_alteração"
```    
### 7. Subir uma alteração
**`Sempre que for subir uma alteração, é necessário utilizar um git add antes do commit`**

```Git
git add .
git commit -m "alteração_do_arquivo"
```    

### 8. Git Log
**`Retorna todas as versões do projeto`**
Todo commit possui um Hash (código referente ao commit)
HEAD indica em qual versão do projeto estamos
```Git
git log
```  
Para sair do git log
```Git
q
```  

### 9. Git Checkout
Volta o projeto para uma versão anterior
Para isso, digite os seis primeiros dígitos do hash do commit que deseja voltar

```Git
git chekcout digitos_hash
```  

Para isso digite o comando 
    git init
    git add .
    git commit -m "nome da alteração"
    git branch -M main
    git remote add origin 'link do repositório'
    git push (envia)
    git pull (puxa do github)

Como criar um arquivo que não vai ser enviado pelo git
    .gitignore