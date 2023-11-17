# Use a imagem do node versão 16 alpine
FROM node:16-alpine3.11

# Exponha a porta 3001
EXPOSE 3001

# Defina o diretório de trabalho para /app/back-end
WORKDIR /app/back-end

# Adicione o arquivo node_modules.tar.gz à imagem e descompacte-o
ADD ./node_modules.tar.gz ./

# Copie todos os arquivos da pasta back-end para a imagem
COPY . .

ENTRYPOINT [ "npm" ]

# Inicie a aplicação com o comando npm start
CMD ["start"]