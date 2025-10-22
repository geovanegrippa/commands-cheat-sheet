# 🧭 Principais Comandos Git e GitHub

---

## 📘 1. Conceitos Básicos

| Termo | Descrição |
|-------|------------|
| **Git** | Sistema de controle de versão distribuído usado para rastrear alterações em código. |
| **GitHub** | Plataforma de hospedagem de código baseada em Git. |
| **Repositório (repo)** | Local onde o código e o histórico de versões são armazenados. |
| **Commit** | Registro de uma ou mais alterações no código. |
| **Branch** | Linha de desenvolvimento separada dentro do repositório. |
| **Merge** | Combina alterações de uma branch em outra. |
| **Pull Request (PR)** | Solicitação para mesclar alterações no GitHub. |

---

## ⚙️ 2. Configuração Inicial

```bash
# Define o nome do usuário
git config --global user.name "Seu Nome"

# Define o e-mail do usuário
git config --global user.email "seuemail@example.com"

# Verifica as configurações atuais
git config --list
```

---

## 🏗️ 3. Criação e Clonagem de Repositórios

```bash
# Inicializa um novo repositório Git
git init

# Clona um repositório existente
git clone https://github.com/usuario/nome-do-repositorio.git
```

---

## 📂 4. Controle de Versão (Arquivos e Commits)

```bash
# Mostra o status das alterações
git status

# Adiciona um arquivo específico para commit
git add arquivo.txt

# Adiciona todas as alterações
git add .

# Faz o commit com uma mensagem
git commit -m "Mensagem descritiva do commit"

# Exibe o histórico de commits
git log

# Mostra diferenças entre o que foi alterado e o último commit
git diff
```

---

## 🌿 5. Branches

```bash
# Lista todas as branches
git branch

# Cria uma nova branch
git branch nome-da-branch

# Muda para uma branch existente
git checkout nome-da-branch

# Cria e muda para uma nova branch
git checkout -b nome-da-branch

# Faz merge da branch atual com outra
git merge nome-da-branch

# Deleta uma branch local
git branch -d nome-da-branch
```

---

## 🔁 6. Sincronização com o GitHub

```bash
# Adiciona o repositório remoto
git remote add origin https://github.com/usuario/nome-do-repositorio.git

# Envia alterações para o GitHub
git push origin nome-da-branch

# Faz o primeiro push e define a branch padrão
git push -u origin main

# Baixa as alterações mais recentes do repositório remoto
git pull

# Atualiza informações do repositório remoto sem merge automático
git fetch
```

---

## 🧹 7. Revertendo e Corrigindo Alterações

```bash
# Desfaz mudanças em um arquivo antes do commit
git restore arquivo.txt

# Remove arquivos do staging area
git reset arquivo.txt

# Reverte o último commit (mantém alterações)
git reset --soft HEAD~1

# Reverte o último commit (descarta alterações)
git reset --hard HEAD~1

# Reverte um commit específico (gera novo commit inverso)
git revert <hash_do_commit>
```

---

## 👥 8. Colaboração e Pull Requests

### 🔹 Criando um Pull Request no GitHub

1. Faça o push da sua branch:
   ```bash
   git push origin nome-da-branch
   ```
2. No GitHub, clique em **Compare & Pull Request**.  
3. Adicione título e descrição das alterações.  
4. Solicite **review** (opcional) e clique em **Create Pull Request**.

---

## 🧠 9. Comandos Úteis Extras

```bash
# Mostra o repositório remoto configurado
git remote -v

# Renomeia uma branch
git branch -m nome-antigo nome-novo

# Remove um repositório remoto
git remote remove origin

# Mostra quem alterou cada linha de um arquivo
git blame nome-do-arquivo

# Mostra as diferenças entre duas branches
git diff branch1..branch2
```

---

## 🧱 10. Fluxo de Trabalho Padrão (Workflow)

```bash
# 1️⃣ Clonar o repositório
git clone https://github.com/empresa/projeto.git

# 2️⃣ Criar uma nova branch para sua feature
git checkout -b feature/nome-da-feature

# 3️⃣ Fazer alterações e commit
git add .
git commit -m "Implementa nova funcionalidade X"

# 4️⃣ Enviar a branch para o GitHub
git push origin feature/nome-da-feature

# 5️⃣ Criar Pull Request no GitHub
```

---

## 🏁 11. Boas Práticas

✅ Use **mensagens de commit claras e objetivas**  
Exemplo:
```bash
git commit -m "Corrige bug na validação de login"
```

✅ Crie **branches separadas** para cada feature ou correção.  
✅ Sempre faça **pull** antes de começar uma nova alteração.  
✅ Faça **code review** antes de dar merge na `main` ou `master`.  
✅ Utilize **.gitignore** para evitar subir arquivos desnecessários.

---

## 📚 12. Referências Úteis

- [Documentação oficial do Git](https://git-scm.com/doc)  
- [Documentação do GitHub](https://docs.github.com/)  
- [Git Cheatsheet by GitHub](https://education.github.com/git-cheat-sheet-education.pdf)

---

💡 **Dica:**  
Para verificar visualmente o histórico de commits e merges:
```bash
git log --oneline --graph --decorate --all
```

---

✍️ **Autor:** Geovane Grippa  
📅 **Última atualização:** Outubro de 2025  
📂 **Licença:** MIT

---
