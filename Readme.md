Git

Este é um repositorio teste para testar o git!

Don't mind me...

// comandos uteis

git config --global user.name "Andre Vaccari"

git config --global user.email "andrevaccari95@gmail.com"

git config --global core.editor code

// comandos uteis

git status // informa a situação atual da pasta

git log // mostra o historico do que foi feito
git log --decorate // melhores infos, branchs...
git log --author="" // filtra autores
git log --graph // mostra de forma grafica

git shortlog // mostra menos detalhadamente os commits
git shortlog -sn // mostra apenas a qtde de commits e a pessoa

git show #commit-hash# // mostra detalhadamente o commit

git diff // mostra as diferenças nos arquivos do projeto com os arquivos commitados
git diff --name-only // mostra apenas uma lista com o nome dos arquivos diferentes dos commitados

git checkout #nome-do-arquivo# // Retorna o arquivo ao estado do ultimo commit

git reset HEAD #nome-do-arquivo# // tira o arquivo da fila do STAGE

git reset --soft // pega as modificações e volta, mas o arquivo fica pronto para ser commitado novamente
git reset --mixed // pega as modificações e volta, mas o arquivo para antes do STAGE
git reset --hard // ignora a existencia do commit e reseta o arquivo para antes dele

git remote add #nome-remoto(padrão => origin)# #link-do-repositorio-remoto#

git remote // mostra os repositorios remotos adicionados
git remote -v // mostra os repositorios remotos com endereço

git push -u origin master // primeiro push. -u serve para tornar o "push origin master" padrão. "origin => pra onde vai" "master => de onde vem"

git checkout #nome-do-branch# // muda para o branch ja criado
git checkout -b #nome-do-branch# // criar novo branch no repositório

git branch // mostra todos os branchs no repositório, * no atual
git branch -D #nome-do-branch# // Deleta o branch