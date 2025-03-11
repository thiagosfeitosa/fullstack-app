# Usar a última versão LTS do Node.js
FROM node:lts

# Definir diretório de trabalho dentro do container
WORKDIR /workspace

# Atualizar pacotes e instalar dependências do sistema
RUN apt-get update && apt-get install -y \
    curl git httpie && apt-get clean

# Instalar pacotes globais do Node.js
RUN npm install -g \
    pm2 \
    nodemon \
    yarn \
    eslint \
    prettier \
    graphql-cli \
    jest \
    vitest \
    playwright \
    jwt-cli

# Expor portas para o servidor e frontend
EXPOSE 3000 4000

# Comando padrão do container
CMD ["bash"]