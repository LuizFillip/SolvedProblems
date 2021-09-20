# Abra os arquivos do Jupyter Notebook salvos na pasta Google Drive

por John White
link original: https://hometechtime.com/open-jupyter-notebook-files-saved-in-google-drive-file-stream/

## Problema (John)

Então, recentemente mudei do DropBox para o Google Drive e o processo foi realmente tranquilo, 
até que não consegui acessar nenhum dos meus arquivos .ipynb do Jupyter Notebook por meio do navegador 
de arquivos Jupyter que faz parte da configuração do Anaconda

## Solução

### Etapa 1: Abra o Prompt de Comando (CMD) 

### Etapa 2: Pesquise os seguintes passos

Pesquise o nome do usário local (no meu caso "LuizF") e copie o caminho do diretório 
("C:\Users\LuizF"). Pesquise a Letra da unidade do google drive (no meu caso G:)

### Etapa 3: Faça a junção de diretório

Nesta etapa é necessário um comando que criará uma junção entre seu Google Drive e sua 
estrutura de arquivo regular em sua unidade C: (que o explorador de arquivos jupyter pode ver). 

A junção terá a forama de uma pasta chamada Google Drive, localizada no diretório do usuário do 
Windows.

Comando: mklink /J "C:\Users\LuizF\Google Drive" "G:\"
Saída: Junção criada para C:\Users\LuizF\Google Drive <<===>> G:\

Obs: Coloque cada parte do comando um espaço, caso contrário, dará erro. 
Pelo 'Anaconda prompt' não funcionou, pelo menos para mim.  