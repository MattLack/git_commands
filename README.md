# List of git commands to consult


## Commits 

#### Reseta a branch para o estado do último commit
> Git reset --hard

#### Adiciona os arquivos para staged
> Git add *

#### Comita os arquivos staged
> Git commit -m "<mensagem_de_comit>"

#### Push para upstream
> Git push

#### Pull do Upstream (se estiver em outro branch ele da pull neste branch)
> Git pull
 
#### Merge do local com upstream passado como parêmetro
> git merge origin/<upstream_branch_Name>

#### Clonar de um branch específico
> git clone -b nome_do_branch http://....linkdorepositório

## Branches

####  verifica o status do repositório local e informa qual o branch atual e qual o branch do upstram do remoto
> Git status

#### lista todos os branch mapeados localmente
> Git branch -a

#### atualiza lista de branch existentes no remoto
> Git fetch -p

#### muda para um branch local ou cria um novo caso não exista
> Git  checkout <nome_branch>

#### renomeia um branch
> Git branch -m <nome-antigo> <novo-nome>

#### mostra o nome do remoto
> Git remote -v

#### identifica qual o branch no remoto receberá os commits do repositório
> Git branch <local-branch> -u <remote>/<remote-branch>

## Upar projeto
```
git init
git add .
git commit -m "First commit"
git remote add origin <remote repository URL>
git remote -v
git push -f origin master
```
-----------------------------------------------------------------------------------------------------------------------------------
	
							Ordem geral para comitar mudanças no seu código
							
0 - git status (para visualizar os arquivos modificados)
1 - git add .
2 - git commit -m "texto para titulo do commit"
3 - git push

-----------------------------------------------------------------------------------------------------------------------------------

-- para fazer push de um branch para outro
git push origin seu_branch_atual:o_outro_branch

_______________________________________________________________________________________________________________________________________

--visualizar os arquivos que estão com conflito
git diff --name-only --diff-filter=U

-- resolver problema para criação do primeiro branch 
git checkout -t -b master origin/master

________________________________________________________________________________________________________________________________________

git init 
inicializa um repositório git local vazio

mkdir {project}
cd {project}
git init

git status
verifica o status do seu branch local

git add {file}
Adiciona arquivo a fila de itens modificados no branch

echo {mensagem} > {file}
Adiciona a mensagem/texto ao arquivo

touch {file.extension}
Cria arquivo na extensão dentro do branch

git add .
Adiciona todos os arquivos modificados e criados no branch a lista de itens do branch 

git commit -m "{mensagem}"
Captura um Snapshot dos arquivos adicionados a lista de itens (tira como uma foto desse momento do branch)

git --version
Verifica a versão do git que está instalada em seu computador

git log
Verifica o histórico dos commits do branch em um único hash code

git show {point}
Mostra informações sobre o commit relacionado ao point

git checkout {hash code}
Atualiza o workstation do seu diretório local para o commit com o hash code repassado 

git checkout {branch}
Atualiza o workstation do seu diretório local para o último commit do branch

git tag {version}
Auxilia no gerenciamento de versão dos commits criando uma tag para utilizar no lugar do hash code


