# Git Commands

#### Este é um repositorio com os comandos GIT!

## Configurações Globais

* git config --global user.name "_username_"
* git config --global user.email "_email_"
* git config --global core.editor code

## Comandos

1. __git status__ // informa a situação atual da pasta

2. __git log__ // mostra o historico do que foi feito
    1. git log --decorate // melhores infos, branchs...
    2. git log --author="_username_" // filtra autores
    3. git log --graph // mostra de forma grafica

3. __git shortlog__ // mostra menos detalhadamente os commits
    1. git shortlog -sn // mostra apenas a qtde de commits e a pessoa

4. __git show__ _commit-hash_ // mostra detalhadamente o commit

5. __git diff__ // mostra as diferenças nos arquivos do projeto com os arquivos commitados
    1. __git diff --name-only__ // mostra apenas uma lista com o nome dos arquivos diferentes dos commitados

6. __git checkout__ _nome-do-arquivo_ // Retorna o arquivo ao estado do ultimo commit

7. __git reset HEAD__ _nome-do-arquivo_ // tira o arquivo da fila do STAGE
    1. __git reset --soft__ _commit-hash_ // pega as modificações e volta, mas o arquivo fica pronto para ser commitado novamente
    2. __git reset --mixed__ _commit-hash_ // pega as modificações e volta, mas o arquivo para antes do STAGE
    3. __git reset --hard__ _commit-hash_ // ignora a existencia do commit e reseta o arquivo para antes dele

8. __git remote add__ _nome-remoto(padrão => origin)_ _link-do-repositorio-remoto_

9. __git remote__ // mostra os repositorios remotos adicionados
    1. __git remote -v__ // mostra os repositorios remotos com endereço

10. __git push -u origin master__ // primeiro push. -u serve para tornar o "push origin master" padrão. "origin => pra onde vai" "master => de onde vem"

11. __git checkout__ _nome-do-branch_ // muda para o branch ja criado
    1. git checkout -b _nome-do-branch_ // criar novo branch no repositório

12. __git branch__ // mostra todos os branchs no repositório, * no atual
    1. __git branch -D__ _nome-do-branch_ // Deleta o branch
