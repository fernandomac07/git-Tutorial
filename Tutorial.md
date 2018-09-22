## TUTORIAL git


## CONFIGURANDO O git

# Configurando o nome do usuário do git
git config --global user.name "Nome do usuário"

# Configurando Email do usuário do git
git config --global user. email "Email do Usuário"

# Configurando o editor
git config --global core.editor "editor de sua preferência"

## CRIANDO UM REPOSITÓRIO NO git

# Criando repositório
mkdir nome do diretório

# Entrando no diretório
cd nome do diretório/

# Incorporando o diretório ao git
git init

## CRIANDO UM ARQUIVO NO git

# Para criar um arquivo no git, é necessário primeiro chamar o editor escolhido como principal nas 
#configurações iniciais (Ex: vim ou Atom), em seguida o nome do arquivo que deseja criar
vim arquivo.md

# Após chamar o comando, você será direcionado para a tela do editor de texto escolhido.
# Para começar uma edição é necessario apertar a trcla (i) para iniciar o modo de edição
# após ter adicionado ou modificado as informações no arquivo apertamos a tecla (Esc) para
#sair do modo de edição, em seguida apertar a tecla (:), seguido da tecla (w) para salvar as
#alterações e depois a tecla (q) para fechar o editor de testo e retornar ao console do git

# STATUS DOS ARQUIVOS

# No git os arquivos podem estar em 3 status diferentes (Untracked, modified ou Unstage)

# untracked = quando você cria o arquivo mas o git ainda não o reconhece
# modified = quando você modifica o arquivo
# unstage = quando o arquivo está na sua fase final, pronto para ser comitado (criar uma verção)

# Identificando o status do arquivo
git status

# quando você não tem nada de informação o git status aparecerá untracked
# para mudar o status do arquivo é preciso adicionar o arquivo no diretório do git
git add nome do arquivo.md

# após executar este comando o status mudará para unstage, ou seja está pronto para ser comitado
# caso você resolva modificar o arquivo, o status dele irá para modified, então será necessário adiciona-lo
# novamente para que o status retorne para unstage e assim ser comitado (salvo)

# Comitando arquivo (salvando uma versão)
git commit -m "Mensagem"

# O argumento utilizado no comando git commit (-m) serve para você adicionar um comentário na versão que foi salva
# É bastante comum se adicionar nos comentários o que foi modificado na versão, assim facilita para que outros usuários saibam 
#o que foi feito na versão.

## VISUALIZANDO O HISTÓRICO DOS COMMITES

# Para visualizar as modofocações que foram feitas nas versões utilizamos o (git log)
git log

# Este comando tem várias funcionalidades podendo resumir os dados a serem observados

git log --decorate
# o git log -- decorate mostra de onde veio o arquivo

git log --author "nome do autor"
# filtra os commites pelos autores das versões

git shortlog
# mostra uma lista em ordem alfabética com todos os autores, número de commites e quais foram eles

git shortlog -sn
# Mostra apenas a quantidade de commites e os autores

git log --graph
# mostra em uma forma gráfica o que está ocorrendo com as modificações dos arquivos

# Visualizando as modificações dos commites através da rash. Para isso é necessário copiar a rash referente ao commite a ser observado
#e inserir no comando git show
git show rash do commite

## OBSERVANDO AS MODIFICAÇÕES ANTES DE CRIAR UM COMMITE

# Vizualizando as Modificações antes de salvar as versões
git diff

