# 📘 Principais Comandos do Git + Boas Práticas de Commits

Este guia reúne os comandos mais usados no Git e suas funções, além de boas práticas de mensagens de commit, ideal para estudo da certificação **GH-900**.

---

## 📌 Comandos Básicos

| Comando | Função | Exemplo |
|---------|--------|---------|
| `git init` | Cria um novo repositório Git no diretório atual. | `git init` |
| `git clone [URL]` | Copia um repositório remoto para sua máquina local. | `git clone https://github.com/user/repo.git` |
| `git status` | Mostra o estado atual do repositório: arquivos modificados, rastreados e não rastreados. | `git status` |
| `git add [arquivo]` | Adiciona arquivos à área de preparação (staging). | `git add index.html` |
| `git commit -m "mensagem"` | Salva as alterações no histórico do repositório com uma mensagem descritiva. | `git commit -m "Corrige bug de login"` |
| `git log` | Exibe o histórico de commits. | `git log` |
| `git diff` | Mostra diferenças entre versões de arquivos. | `git diff` |

---

## 🌿 Branches e Navegação

| Comando | Função | Exemplo |
|---------|--------|---------|
| `git branch` | Lista branches existentes ou cria uma nova branch. | `git branch nova-feature` |
| `git checkout [branch]` | Troca para outra branch. | `git checkout main` |
| `git switch [branch]` | Alternativa moderna ao checkout para mudar de branch. | `git switch dev` |
| `git merge [branch]` | Mescla alterações de uma branch em outra. | `git merge nova-feature` |
| `git rebase [branch]` | Reaplica commits sobre outra branch, mantendo histórico linear. | `git rebase main` |

---

## 🔄 Repositórios Remotos

| Comando | Função | Exemplo |
|---------|--------|---------|
| `git remote -v` | Lista os repositórios remotos configurados. | `git remote -v` |
| `git push [remote] [branch]` | Envia commits locais para o repositório remoto. | `git push origin main` |
| `git pull [remote] [branch]` | Atualiza o repositório local com mudanças do remoto. | `git pull origin main` |
| `git fetch` | Baixa alterações do remoto sem mesclar automaticamente. | `git fetch origin` |

---

## 🛠️ Outros Comandos Úteis

- `git reset [arquivo]` → Remove arquivo da área de preparação.  
- `git reset --hard [commit]` → Volta o repositório para um commit específico, descartando alterações.  
- `git stash` → Guarda temporariamente alterações não commitadas.  
- `git tag [nome]` → Marca commits importantes (ex.: versões).  
- `git config --global user.name "Seu Nome"` → Configura identidade do usuário.  
- `git help [comando]` → Exibe ajuda detalhada sobre um comando.  

---

## ✍️ Boas Práticas de Commits

Segundo o artigo [The Art of Writing Meaningful Git Commit Messages](https://medium.com/@iambonitheuri/the-art-of-writing-meaningful-git-commit-messages-a56887a4cb49), escrever commits claros é essencial para colaboração em equipe e manutenção futura.  

### Estrutura de um bom commit
- **Simples:** `git commit -m "<mensagem>"`  
- **Detalhado:** `git commit -m "<título>" -m "<descrição>"`  
- **Amend:** `git commit --amend` → corrige ou complementa o último commit (evite em commits já públicos).  

### Convenção de tipos (Conventional Commits)
- **feat:** nova funcionalidade  
- **fix:** correção de bug  
- **docs:** documentação  
- **style:** formatação sem impacto no código  
- **refactor:** refatoração sem adicionar feature ou corrigir bug  
- **test:** inclusão ou ajuste de testes  
- **chore:** manutenção (dependências, configs)  
- **perf:** melhorias de performance  
- **ci:** integração contínua  
- **build:** mudanças em sistema de build  
- **ops:** infraestrutura, deploy, backup  
- **revert:** desfaz um commit anterior  

### Regras para mensagens
- Limite o título a **50 caracteres**  
- Use **imperativo** (“add”, “fix”, “update”)  
- Separe título e corpo com uma linha em branco  
- Corpo explicativo com **o que** e **por que**  
- Quebre linhas do corpo em **72 caracteres**  


---

## 🎯 Dicas para a prova GH-900

- Memorize a diferença entre **git add** (preparar) e **git commit** (salvar).  
- Entenda bem **branch, merge e rebase**, pois são cobrados em questões práticas.  
- Saiba distinguir **pull** (traz e mescla) de **fetch** (traz sem mesclar).  
- Use **git status** constantemente para acompanhar o que está acontecendo.  
- Pratique escrever commits com **convenções padrão** para ganhar pontos extras em boas práticas.  

---

✍️ Autor: @SteAmarante  
📖 Referência: [The Art of Writing Meaningful Git Commit Messages (Medium)](https://medium.com/@iambonitheuri/the-art-of-writing-meaningful-git-commit-messages-a56887a4cb49)

