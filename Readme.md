# Git Commands

#### Este é um repositorio com os comandos GIT!

## Configurações Globais

* git config --global user.name "_username_"
* git config --global user.email "_email_"
* git config --global core.editor code

## Comandos

1. __git status__ // informa a situação atual da pasta

2. git log // mostra o historico do que foi feito
  1. git log --decorate // melhores infos, branchs...
  2. git log --author="_username_" // filtra autores
  3. git log --graph // mostra de forma grafica

3. git shortlog // mostra menos detalhadamente os commits
  1. git shortlog -sn // mostra apenas a qtde de commits e a pessoa

4. git show _commit-hash_ // mostra detalhadamente o commit

5. git diff // mostra as diferenças nos arquivos do projeto com os arquivos commitados
  1. git diff --name-only // mostra apenas uma lista com o nome dos arquivos diferentes dos commitados

6. git checkout _nome-do-arquivo_ // Retorna o arquivo ao estado do ultimo commit

7. .git reset HEAD _nome-do-arquivo_ // tira o arquivo da fila do STAGE
  1. git reset --soft // pega as modificações e volta, mas o arquivo fica pronto para ser commitado novamente
  2. git reset --mixed // pega as modificações e volta, mas o arquivo para antes do STAGE
  3. git reset --hard // ignora a existencia do commit e reseta o arquivo para antes dele

8. git remote add _nome-remoto(padrão => origin)_ _link-do-repositorio-remoto_

9. git remote // mostra os repositorios remotos adicionados
  1. git remote -v // mostra os repositorios remotos com endereço

10. git push -u origin master // primeiro push. -u serve para tornar o "push origin master" padrão. "origin => pra onde vai" "master => de onde vem"

11. git checkout _nome-do-branch_ // muda para o branch ja criado
  1. git checkout -b _nome-do-branch_ // criar novo branch no repositório

12. git branch // mostra todos os branchs no repositório, * no atual
  1. git branch -D _nome-do-branch_ // Deleta o branch