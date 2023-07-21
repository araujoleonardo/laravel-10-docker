FROM node:18-alpine

# Atualiza o npm para a versão mais recente
RUN npm install -g npm

# Instala o Vue CLI globalmente
RUN npm install -g @vue/cli

# Copiar o arquivo package.json e package-lock.json
COPY package*.json ./

# Instalar as dependências do projeto
RUN npm install

# Copiar o restante dos arquivos do projeto para o container
COPY . .

# Compilar a aplicação Vue.js para produção
#RUN npm run build