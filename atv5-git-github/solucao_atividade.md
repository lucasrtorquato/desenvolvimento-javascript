# Passo 1: Criação da pasta 'desenvolvimento-javascript'
"Criando a pasta 'desenvolvimento-javascript'..."
mkdir desenvolvimento-javascript
cd desenvolvimento-javascript

# Passo 2: Inicializando o repositório Git
"Inicializando o repositório Git..."
git init

# Passo 3: Configurando nome e e-mail no Git (se ainda não configurado)
"Configurando nome e e-mail no Git..."
git config --global user.name "Seu Nome"
git config --global user.email "seuemail@example.com"

# Passo 4: Criando o arquivo README.md com descrição
"Criando o arquivo README.md..."
"# Desenvolvimento JavaScript" > README.md

# Passo 4: Criando o arquivo anotacoes.txt com informações sobre JavaScript
"Criando o arquivo anotacoes.txt..."
"JavaScript é uma linguagem de programação usada para criar páginas web interativas." > anotacoes.txt

# Passo 5: Adicionando os arquivos ao controle de versão e fazendo o commit
"Adicionando os arquivos ao Git..."
git add README.md anotacoes.txt
git commit -m "Adiciona README e anotacoes sobre JavaScript"

# Passo 5: Criando repositório remoto no GitHub e conectando (substitua pelo seu URL do GitHub)
"Conectando ao repositório remoto no GitHub..."
git remote add origin https://github.com/seuusuario/desenvolvimento-javascript.git

# Passo 6: Enviando o commit para o repositório remoto
"Enviando o commit para o GitHub..."
git branch -M main
git push -u origin main

# Passo 7: Editando o arquivo anotacoes.txt e fazendo o commit
"Editando o arquivo anotacoes.txt..."
"JavaScript é uma das linguagens mais populares para desenvolvimento web." >> anotacoes.txt
git add anotacoes.txt
git commit -m "Adiciona mais informações sobre JavaScript no anotacoes.txt"
git push origin main

# Passo 8: Excluindo a pasta local e clonando novamente do GitHub
"Excluindo a pasta local e clonando o repositório novamente..."
cd ..
rm -rf desenvolvimento-javascript
git clone https://github.com/seuusuario/desenvolvimento-javascript.git

# Passo 9: Adicionando seu nome ao final do arquivo anotacoes.txt e enviando para o GitHub
cd desenvolvimento-javascript
"Nome do usuário: Seu Nome" >> anotacoes.txt
git add anotacoes.txt
git commit -m "Adiciona nome no final do arquivo anotacoes.txt"
git push origin main

# Extra - Passo 10: Adicionar estrutura das atividades já realizadas no curso e enviadas pelo Google Classroom
Criar as pastas e adicionar os arquivos
git add .
git commit -m "Criação de pastas com atividades já realizadas e enviadas via Google Classroom"
git push origin main
