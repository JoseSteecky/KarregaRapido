# KarregaRapido
Inicialmente é necessário definir a configuração do git na sua máquina para garantir que todas as contribuições que vier a fazer ao projeto lhe sejam creditadas e receba a nota final que deveras lhe corresponde, para isso deve executar git config --global user.name "José dos Anzóis" seguido de git config --global user.email JoseAnzois@tecnico.ulisboa.pt. Este email deve coincidir com o que tem registado no GItHub, Para mais informação pode consultar https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup


Deve de seguida criar uma cópia local do repositório remoto com o comando git clone https://github.com/JoseSteecky/KarregaRapido


Fazendo git status pode ver que o repositório local está no branch master


Na linha de comando do git fazer git add <file.extention>, para adicionar o ficheiro ao conjunto de ficheiros a ser incluído no próximo commit, é incluído na staging area
Na linha de comando do git fazer git commit -m "group member info added to README.md", para fazer commit local das alterações existentes na área de staging area

Antes de enviar as alterações para o repositório remoto é conveniente garantir que se tem a sua versão mais atual, para isso deve-se fazer git fetch origin

Se o repositório remoto possui alterações que ainda não existem localmente é necessário integrá-las localmente, para isso deve ser feito um merge entre a informação local e a remota executando git merge origin master

No caso de haver conflitos, o que ocorrerá no ficheiro README.md se algum dos colegas já tiver atualizado o repositório remoto, é necessário resolver os conflitos, para isso deve abrir o ficheiro no Eclipse, o icon d ficheiro tem a indicação que possui um conflito, e altera-se o ficheiro para integrar as alterações. Os locais de conflito são indicados por <<<<<<<< HEAD, ========, e >>>>>>>> refs/remotes/origin/master

É necessário voltar a adicionar o ficheiro alterado à staging area fazendo git add README.md
Efetuar um novo commit, git commit -m "conflict resolution", que agora com o ficheiro integrado
E, finalmente, colocar as alterações no repositório remoto, git push origin master
Durante este processo pode-se ir vendo o estado atual com git status
