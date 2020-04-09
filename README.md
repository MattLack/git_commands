# List of git commands to consult

```
mkdir {project}
cd {project}
git init
```

## Ordem geral para comitar mudanças no seu código
```							
0 - git status (para visualizar os arquivos modificados)
1 - git add .
2 - git commit -m "texto para titulo do commit"
3 - git push
```
==========================================================================

## Upar projeto
```
git init
git add .
git commit -m "First commit"
git remote add origin <remote repository URL>
git remote -v
git push -f origin master
```
==========================================================================

## Commits 

#### Reseta a branch para o estado do último commit
```
git reset --hard
```
#### Adiciona os arquivos para staged
```
git add *
```
#### Comita os arquivos staged
```
git commit -m "<mensagem_de_comit>"
```
#### Push para upstream
```
git push
```
#### Pull do Upstream (se estiver em outro branch ele da pull neste branch)
```
git pull
``` 
#### Merge do local com upstream passado como parêmetro
```
git merge origin/<upstream_branch_Name>
```
#### Clonar de um branch específico
```
git clone -b nome_do_branch http://....linkdorepositório
```
#### Checar configurações locais do git
```
git config --list
```
## Branches

####  verifica o status do repositório local e informa qual o branch atual e qual o branch do upstram do remoto
```
git status
```
#### lista todos os branch mapeados localmente
```
git branch -a
```
#### atualiza lista de branch existentes no remoto
```
git fetch -p
```
#### muda para um branch local ou cria um novo caso não exista
```
git checkout <nome_branch>
```
#### renomeia um branch
```
git branch -m <nome-antigo> <novo-nome>
```
#### mostra o nome do remoto
```
git remote -v
```
#### identifica qual o branch no remoto receberá os commits do repositório
```
git branch <local-branch> -u <remote>/<remote-branch>
```
==========================================================================


#### para fazer push de um branch para outro
```
git push origin seu_branch_atual:o_outro_branch
```
#### visualizar os arquivos que estão com conflito
```
git diff --name-only --diff-filter=U
```
#### resolver problema para criação do primeiro branch 
```
git checkout -t -b master origin/master
```

==========================================================================

#### inicializa um repositório git local vazio
```
git init 
```
#### verifica o status do seu branch local
```
git status
```
#### Adiciona arquivo a fila de itens modificados no branch
```
git add {file}
```
#### Adiciona a mensagem/texto ao arquivo
```
echo {mensagem} > {file}
```
#### Cria arquivo na extensão dentro do branch
```
touch {file.extension}
```
#### Adiciona todos os arquivos modificados e criados no branch a lista de itens do branch 
```
git add .
```
#### Captura um Snapshot dos arquivos adicionados a lista de itens (tira como uma foto desse momento do branch)
```
git commit -m "{mensagem}"
```
#### Verifica a versão do git que está instalada em seu computador
```
git --version
```
#### Verifica o histórico dos commits do branch em um único hash code
```
git log
```
#### Mostra informações sobre o commit relacionado ao point
```
git show {point}
```
#### Atualiza o workstation do seu diretório local para o commit com o hash code repassado 
```
git checkout {hash code}
```
#### Atualiza o workstation do seu diretório local para o último commit do branch
```
git checkout {branch}
```
#### Auxilia no gerenciamento de versão dos commits criando uma tag para utilizar no lugar do hash code
```
git tag {version}
```
#### Deletar Branchs
```
git push --delete <remote_name> <branch_name>
git branch -d <branch_name>
```
