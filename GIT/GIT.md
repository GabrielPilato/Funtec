# GIT

- Sistema de controle de versões.

- <h2> COMANDOS BÁSICOS DE PROMPT: </h2>

- dir, Lista os arquivos e pastas do diretório atual; -- Este comando pode listar diretórios fora do atual, adicionar o endereço desejado na frente:
  EXEMPLO: dir C:\Users
  
- cd, Navega até a pasta digitada, 
  EXEMPLO: cd C:\
    -- Este comando nos leva até o C.

- mkdir, é o comando responsável para criar diretórios, o nome do mesmo será o que você digitar na frente,
  É possível criar diretórios em outros diretórios fora do atual
    EXEMPLO: mkdir C:\workspace\teste 
      Este exemplo, cria dentro da pasta workspace, a pasta teste, e caso a pasta workspace não exista, a mesma será criada também
      
 - ">", assim como no Linux, é responsável para encaminhar o resultado de algum comando para um arquivo, normalmente um arquivo TXT.
  EXEMPLO: echo Hello > Hello.txt 
    Este exemplo resultara da criação de um arquivo Hello.txt com o conteúdo "Hello"
 
 - del, Apaga o conteudo de uma pasta
 - rmdir, Apaga o diretório digitado

- INSTALANDO O GIT ATRAVÉS DO SITE OFICIAL https://git-scm.com/
    - Iniciamos o GIT Bash
    
    - <h2> CONFIGURANDO ACESSO </h2>
      - git config --global user.email "gabrielpilato@hotmail.com"
      - git config --global user.name "GabrielPilato"

    - <h2> CONCEITOS DE GIT </h2>
      Blobs - Conteúdos, usados para armazenar
      Trees - A arvore de diretórios, é basicamente um diretório, pode armazenar blobs ou até mesmo outras arvores.
      Commit - O comando de atualização e inserção e exclusão de códigos e arquivos.

    SHA1 - É uma criptografia, uma assinatura contendo todas as informações do commit.

    - <h2> CRIANDO O REPOSÍTÓRIO </h2>
    - git init - Inicia o repositório.
    - git add - Adiciona um arquivo, começa o versionamento de código
    - git commit - Para dar commit nessas alterações realizadas.
      - "-m" adiciona uma mensagem git commit -m "Comentario"
      - "-a" executa tudo que está no stage, inclusive as exclusões.
    - git status - Para identificar a diferença entre o que você colocou na zona de stage e o que está presente no commit anterior

      - git add * , adiciona todos os arquivos pra zona de stage, inclusive, caso haja alguma exclusão de arquivos nesta pasta que estava na versão anterior
      ele também realizará a exclusão,
        - Através do git status é possível identificar o que está sendo adicionado  e o que está sendo deletado.

      - git log , apresenta os commits realizados e dependendo das opções digitadas, mais ou menos informações irão aparecer.
          - git log --oneline, apresenta todos os commits com seus Hash e seus comentários, uma maneira bem simples e organizada de analizar as alterações
          - git log --stat, apresenta todos os commits de forma estatística, mostrando as linhas adicionadas ou excluídas
          - git log -p, apresenta o que exatamente foi adicionado ou excluido, mostrando na tela o código que foi alterado.

      - git restore --stage 'Nome do arquivo', é responsável por tirar certos arquivos da zona de stage e evitar que os mesmos sejam commitados na execução do git commit.
      - git revert numero_hash, quando desejar reverter um commit, é necessário copiar o seu codigo hash e realizar esse comando.
      - git restore --stage 'Nome do arquivo', é o comando responsável por retirar arquivos do stage, ou seja, ele nserá retirado da zona onde será commitado os arquivos.
      - git mv 'nomeArquivo' 'novoNomeArquivo', comando responsável por alterar o nome do arquivo
      - git config --global unset user.email ou user.name, utilizado para retirar o nome e email previamente setados, eles podem ser overwriten também.
      - git config --list, lista as configurações do git, inclusive o nome e o email estarão na lista caso seja necessário verificar

- <h2> VINCULANDO O GIT AO GITHUB </h2>
- git remote add origin 'link http', esse link consegue ser copiado no botão "code" na pagina inicial do repositório.
- git remote -v
- git push origin master, este comando envia o que está no nosso diretório local para o diretório remoto

- git pull origin master, este comando tras do diretório remoto e coloca no diretório local

    No ato de um conflito de versões entre o github (repositório remoto) e o repositório local, o git apontara uma divergência e dentro do arquivo
  ele adicionará linhas de código identificando as linhas com divergências, então é necessário alterar e decidir uma versão final para ser definida tanto no local quanto
  no remoto

    
