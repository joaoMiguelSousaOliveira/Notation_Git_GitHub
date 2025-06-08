# GitHub

### 1. Na página do Projeto
**`Chegue nela via terminal utilizando cd`**

### 2. Conete o seu projeto à sua url do GitHub
**`Adicione ao seu repositório uma versão remota`**
```Git
git remote add origin sua_url.git
``` 

### (Opcional). Mude o nome do Branch
**`Recomenda-se que o nome do branch principal seja main`**
```Git
git branch -m main
```  

### 3. Enviar conteúdos da branch para o repositório
**`Envia os conteúdos da main para o repositório remoto principal`**
```Git
git push -u origin main
```  

### 4. Logar com o GitHub
**`Gere um token para logar`**

## Como enviar conteudos de uma branch secundária para o GitHub
**`Após usar o add e o commit estando na branch, deverá utilizar o comando`**
```Git
git push origin nome_da_branch
```  

## Como pegar um repositório do GitHub

### Git Clone
**`Gera um clone do repositório na sua máquina`**

Crie uma pasta no seu computador e digite no terminal o caminho
```Git
git clone url_do_repositorio
```  

## Criar uma cópia de um repositório para sua conta 

### Fork
**`Cria uma um repositório de outro projeto na sua conta`**

Utilizado para projetos de open sorce. 
O fork copia todos os commits e branchs.
```
No repositório do GitHub que deseja dar o fork
Fork
Create Fork
```  


