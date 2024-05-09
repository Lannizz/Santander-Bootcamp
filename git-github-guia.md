## 📚 Git e Github: Um Guia Prático 🚀 

Este documento apresenta um resumo dos comandos e conceitos básicos do Git e Github, ferramentas essenciais para versionamento de código e colaboração em projetos de software. 

---
## 🧬 Git 

O Git é um Sistema de Versão Distribuído (SVD) que permite rastrear alterações em arquivos ao longo do tempo e colaborar com outros desenvolvedores em projetos de software. 

## 🐙 Github

Github é uma plataforma de hospedagem de código que usa Git para controle de versão e facilita a colaboração em projetos.

**Fluxo de Trabalho Básico:**

### ➡️ Enviando alterações para o repositório remoto:

1. **`git init`** - Inicia um repositório Git na pasta atual.
2. **`git branch -M main`** - Define o nome da branch principal como "main".
3. **`git remote add origin <URL_do_repositório>`** - Conecta o repositório local ao repositório remoto que você criou no Github.
4. **`git status`** - Mostra o status dos arquivos (se estão ou não adicionados ao stage).
5. **`git add <nome_do_arquivo>` (ou `git add .` para adicionar todos)** - Adiciona os arquivos ao stage.
6. **`git commit -m "Mensagem do commit"`** - Salva as alterações no repositório local com uma mensagem.
7. **`git push -u origin main`** - Envia as alterações do repositório local para o repositório remoto no Github.


### ⬅️  Baixando alterações do repositório remoto:

* **`git pull`** - Baixa e mescla as alterações do repositório remoto para o repositório local.


---
## 🌿 Branchs ("Versões")

Uma branch é uma ramificação independente do seu projeto, um ambiente isolado para fazer alterações e testar novas funcionalidades sem afetar a branch principal. 

**Analogia:** Imagine uma árvore. O tronco principal é a branch "main", e cada galho representa uma branch diferente. Você pode criar novas branchs a partir do tronco ou de outros galhos, e cada branch tem sua própria linha de desenvolvimento independente.

**Comandos de Branch:**

* **`git branch -v`** - Lista todas as branchs e o último commit de cada uma.
* **`git checkout -b <nome_da_nova_branch>`** - Cria uma nova branch e muda para ela.
* **`git checkout <nome_da_branch>`** - Muda para uma branch existente.
* **`git branch -d <nome_da_branch>`** - Exclui uma branch.
* **`git merge <nome_da_branch>`** - Mescla uma branch na branch atual. 


---
## 🛠️ Comandos Úteis:

* **`rm -rf .git`** - Desfaz o `git init` de uma pasta (exclui o diretório .git).
* **`git restore <nome_do_arquivo>`** - Desfaz alterações em um arquivo. 
* **`git commit --amend -m "Nova mensagem"`** - Corrige a mensagem do último commit. 
* **`git reset --soft <código_do_commit>`** - Desfaz o último commit para um commit anterior (use `git log` para ver o código do commit).
* **`git reset <nome_do_arquivo>`** - Remove arquivos da área de stage. 
* **`git fetch origin main`** - Baixa as alterações do repositório remoto sem mesclar com o local.
* **`git diff main origin/main`** - Mostra as diferenças entre o seu repositório local e o remoto.
* **`git merge origin/main`** - Mescla as alterações do repositório remoto com o repositório local.
* **`git clone <URL> --branch <nome_da_branch> --single-branch`** - Clona apenas uma branch específica de um repositório. 
* **`git stash`** - Arquiva alterações temporariamente.
* **`git stash list`** - Lista as alterações arquivadas.
* **`git stash pop`** - Restaura a última alteração arquivada e a remove da lista. 
* **`git stash apply`** - Restaura a última alteração arquivada e a mantém na lista.

---
