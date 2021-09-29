# 1. Especificar a imagem base (obrigatório).
FROM node 

# 2. Definir o diretorio de trabalho da aplicação e copiar os arquivos bases.
WORKDIR /app 

COPY package*.json ./

# 3. Instalar pacotes.
RUN npm install

# 4. Copiar os arquivos auxiliares da app
COPY . .

# 5. Expor a(s) porta(s) que o serviço/app vai utilizar.
EXPOSE 8080 

# 6. Definir o comando de inicialização do container.
CMD ["node", "server.js"] 