# PASSO 1 - PREPARANDO TERRENO PARA WEBPACK

    ## Remover pasta app
    ## Remover system.js importado em index.html
    ## Remover babel do package.json:  ' npm uninstall babel-cli --save-dev '
    ## Remover systemjs do package.json:  ' npm uninstall systemjs --save '
    ## Instalar webpack e babel-core: ' npm install webpack@3.1.0 babel-core@6.25.0 --save-dev '

# PASSO 2 - INDICANDO PRIMEIRO MODULO A SER CARREADO
    ## Criar aquivo: webpack.config.js (É um modulo do node express)

# PASSO 3 - INSTALANDO BABEL-LOADER
    ## Instalar babel-loader: ' npm install babel-loader@7.1.0 --save-dev '
    ## Criar modulo no arquivo de configuração 
        - Incluir regra para o modulo
    ## Remover do arquivo .babelrc : "transform-es2015-modules-systemjs",
    ## Remover dependencias: ' npm uninstall babel-plugin-transform-es2015-modules-systemjs --save-dev '

# PASSO 4 - CRIANDO BUILD DE PRODUÇÃO
    ## Instalar babili: ' npm install babili-webpack-plugin@0.1.1 --save-dev '
    ## Instalar cros-envi ' npm install cross-env@5.0.1 --save-dev ' > Permite execução do build em diferentes
       plataformas.
    ## Adicionar novo script em package.json: ' NODE_ENV=production webpack --config webpack.config.js '
    ## Modificar webpack.config.js
        -  Validar se variavel de ambiente NODE_ENV criada na execução do build é produção, se for 
          'production', irá adicionar uma instancia do bibilinPlugin para minificar o arquivo de build.


# _________________________________________________NOTAS__________________________________________________ #

## DIFERENÇA ENTRE PLUGIN & LOADER
    # LOADER: Trabalha em cada arquivo separado antes do bundle final ser criado.
    # PLUGIN: Trabalha no bundle final

# ________________________________________________________________________________________________________ #


    
