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
