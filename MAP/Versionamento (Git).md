O versionamento de código é o processo de gerenciar as mudanças no código-fonte de um projeto ao longo do tempo. Ele permite que os desenvolvedores acompanhem modificações, colaborem de forme eficiente e revertam para versões antigas se necessário.

# Git e Github
O Git é o sistema de controle de versão distribuído mais usado atualmente. Ele permite criar branches, realizar merges, visualizar o histórico de commits.
O GitHub é a principal plataforma que armazenam repositórios Git na nuvem e facilitam a colaboração.
## Principais comados:
- `git init` → Inicializa um repositório Git.
- `git clone <URL>` → Clona um repositório remoto.
- `git status` → Mostra o status atual dos arquivos.
- `git add <arquivo>` → Adiciona um arquivo ao staging.
- `git commit -m "Mensagem"` → Salva mudanças localmente.
- `git push` → Envia commits para o repositório remoto.
- `git pull` → Atualiza o repositório local com mudanças do remoto.
- `git branch` → Lista/Cria branches.
- `git merge <branch>` → Une branches.

## Mais comandos

### Configuração e inicialização:
- `git config --global user.name "Seu Nome"` → Define o nome do usuário globalmente.
- `git config --global user.email "seu@email.com"` → Define o e-mail do usuário globalmente.
- `git config --list` → Exibe todas as configurações do Git.
- `git init` → Inicializa um novo repositório Git.

### Informações do repositótio:
- `git status` → Mostra o status atual dos arquivos no repositório.
- `git log` → Exibe o histórico de commits.
- `git log --oneline` → Mostra o histórico de commits resumido.
- `git log --graph` → Mostra o histórico em forma de árvore.

### Trabalhando com commits:
- `git add <arquivo>` → Adiciona um arquivo específico ao staging.
- `git add .` → Adiciona todas as mudanças ao staging.
- `git commit -m "Mensagem"` → Confirma as mudanças com uma mensagem.
- `git commit --amend -m "Nova Mensagem"` → Edita o último commit.
- `git reset HEAD <arquivo>` → Remove o arquivo do staging (sem apagar mudanças).

### Branches:
- `git branch` → Lista todas as branches do repositório.
- `git branch <nome-da-branch>` → Cria uma nova branch.
- `git checkout <nome-da-branch>` → Muda para uma branch existente.
- `git checkout -b <nome-da-branch>` → Cria e muda para uma nova branch.
- `git branch -d <nome-da-branch>` → Deleta uma branch local.
- `git branch -D <nome-da-branch>` → Força a exclusão de uma branch local.

### Merge e Rebase:
- `git merge <branch>` → Mescla a branch especificada com a atual.
- `git rebase <branch>` → Move os commits da branch atual para a base da branch especificada.
- `git cherry-pick <commit>` → Aplica um commit específico em outra branch.

### Remote:
- `git remote -v` → Lista os repositórios remotos configurados.
- `git remote add origin <URL>` → Adiciona um repositório remoto.
- `git push -u origin <branch>` → Envia a branch para o repositório remoto.
- `git fetch` → Baixa mudanças do repositório remoto sem aplicá-las.
- `git pull` → Atualiza o repositório local com mudanças do remoto.
- `git push origin --delete <branch>` → Exclui uma branch no repositório remoto.

### Revertendo mudanças:
- `git checkout -- <arquivo>` → Desfaz mudanças em um arquivo não commitado.
- `git reset --soft HEAD~1` → Remove o último commit, mas mantém as mudanças no staging.
- `git reset --mixed HEAD~1` → Remove o último commit e coloca as mudanças no workspace.
- `git reset --hard HEAD~1` → Remove o último commit e apaga as mudanças permanentemente.
- `git revert <commit>` → Cria um novo commit que desfaz as alterações de um commit específico.

### Stash (Salvar Mudanças Temporariamente)

- `git stash` → Salva as mudanças atuais sem commitá-las.
- `git stash pop` → Aplica as mudanças salvas no stash e remove o stash.
- `git stash apply` → Aplica as mudanças do stash, mas mantém a entrada no stash.
- `git stash list` → Lista os stashes armazenados.
- `git stash drop` → Remove um stash específico.

### Tags:
- `git tag` → Lista todas as tags do repositório.
- `git tag -a v1.0 -m "Versão 1.0"` → Cria uma tag anotada com mensagem.
- `git push origin --tags` → Envia as tags para o repositório remoto.
- `git tag -d v1.0` → Deleta uma tag local.
- `git push origin --delete v1.0` → Deleta uma tag no repositório remoto.