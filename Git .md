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
Lembre de control + s antes do git add
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
**`Volta o projeto para uma versão anterior`**

Para isso, digite os seis primeiros dígitos do hash do commit que deseja voltar.
Antes de dar um chekout verificar se há algo para commitar e commite

```Git
git chekcout digitos_hash
```  

### 10. Git Checkout Master
**`Volta para a última versão do projeto`**

```Git
git chekcout master
```  

### Branch

**`Ramificação do projeto principal`** 

Utilizado para trabalho em equipe - **cada desenvolvedor possui a sua branch do projeto**

Toda vez que for ciar uma nova funcionalidade criar uma nova branch 

```Git
git branch nome_do_branch
```  

**`Altera para um branch criado`**

Digite o nome do branch que deseja ir

```Git
git checkout nome_do_branch
```  

**`Altera o nome de um branch`**
Recomenda-se que o branch principal seja chamado de **main**

Para mudar o nome de uma branch, deve estar nele e digitar

```Git
git branch -m novo_nome
``` 


### Pull request
**`Recomenda-se utilizar o merge por meio do pull request`**

O **pull request** é utilizado para evitar conflitos no código da **main**. 

Na prática, ele atua como uma **validação**, que somente após aceita, o código de uma **branch secundária** poderá sofrer o **merge**. Então, ao dar um **push** em uma branch secundária, se o **pull request estiver habilitado**, pode ir em **Pull requests** e em **New pull request** e **ecolher qual branch queremos fazer o merge** (**main->exemplo**). **No pŕoprio pull request, mostra o que o merge da branch selecioanda e da branch que commitamos irá alterar**. O request apresenta os possíveis **`conflitos antes mesmo do merge`**. Os pulls requests podem necessitar da **`aprovação de 1 ou mais desenvolvedores para o merge`**.

**`Como habilitar a opção de pull request`**

```
No repositório:
Settings
Branches
Add branch ruleset
Escolha o nome da ruleset
Require a pull request before merging
Selecione o número de aprovações que desejar
Require approval of the most recent reviewable push
Create
``` 

### Merge

**`Une as Branchs na Branchs principal (main)`**
Deve estar na **branch principal (main)** e utilizar

```Git
git merge nome_do_branch_que_deseja_unir
```

### Git ignore

**`Ignora arquivos selecionados`**

Crie um arquivo **`.gitignore`** contendo os nomes dos arquivos que deseja que o git ignore (**eles não irão subir pro git ou github**)
```
Crie um arquivo chamado .gitgnore
Insira os nomes dos arquivos que deseja ignorar
``` 