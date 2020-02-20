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

### RESUMO ATÉ AQUI ###
- O papel do webpack
- Instalação através do npm
- Configuração do webpack.config.js
- Como executar webpack através de um npm script
- Instalação e configuração de um loader
    
