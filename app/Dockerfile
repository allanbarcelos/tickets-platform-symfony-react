FROM node:18

WORKDIR /app

# Instalar dependências do sistema necessárias para compilação de módulos nativos
RUN apt-get update && apt-get install -y \
    build-essential \
    python3 \
    curl \
    libvips-dev \
    && rm -rf /var/lib/apt/lists/*

# Copiar package.json e package-lock.json (se usar) para instalar as dependências
COPY package*.json ./
RUN npm install

# Copiar o restante do código da aplicação
COPY . .

# Build do Next.js para produção
RUN npm run build

# Expor a porta 3000
EXPOSE 3000

# Comando para iniciar a aplicação no modo produção
CMD ["npm", "start"]
