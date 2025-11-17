# 🚀 EvoGO Manager

[![Node.js](https://img.shields.io/badge/Node.js-18+-green.svg)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-19.1.0-blue.svg)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8+-blue.svg)](https://www.typescriptlang.org/)
[![Docker](https://img.shields.io/badge/Docker-Ready-blue.svg)](https://www.docker.com/)
[![Whatsmeow](https://pkg.go.dev/badge/go.mau.fi/whatsmeow.svg)](https://pkg.go.dev/go.mau.fi/whatsmeow)

Sistema completo de gerenciamento para Evolution GO (whatsmeow), desenvolvido com React + TypeScript + Vite.

## ✨ Funcionalidades

### 📱 Gerenciamento de Instâncias
- Criar, conectar e deletar instâncias WhatsApp
- Gerar QR Code para conexão
- Visualizar status em tempo real (conectado/desconectado)
- Reiniciar e desconectar instâncias
- Gerador automático de tokens seguros
- Copiar ID, Token e JID com um clique

### 💬 Envio de Mensagens
- **Texto:** Mensagens de texto simples
- **Mídia:** Imagens, vídeos e documentos com legenda
- **Áudio:** Envio de áudio/PTT
- **Localização:** Compartilhar coordenadas GPS com nome e endereço

### ⚙️ Configurações Avançadas
- Configurar Webhook URL e eventos
- Always Online (manter sempre online)
- Ignorar grupos
- Ignorar status
- Marcar mensagens como lidas
- Rejeitar chamadas automaticamente

### 📊 Dashboard
- Visão geral de todas as instâncias
- Estatísticas em tempo real
- Taxa de conexão
- Cards informativos com gradientes

## 🛠️ Tecnologias

- **React 18** - Biblioteca UI
- **TypeScript** - Tipagem estática
- **Vite** - Build tool ultra-rápido
- **TailwindCSS** - Estilização
- **shadcn/ui** - Componentes UI modernos
- **React Router** - Navegação
- **TanStack Query** - Gerenciamento de estado
- **Sonner** - Notificações toast
- **Lucide React** - Ícones

## 🔧 Configuração

### Primeiro Acesso

1. Acesse a aplicação
2. Faça login com suas credenciais:
   - **Base URL:** URL da sua Evolution API (ex: `https://evolutiongo.com.br`)
   - **API Key Global:** Sua chave de API global

### Criar Instância

1. Vá para a aba "Instâncias"
2. Preencha o nome da instância
3. Gere um token aleatório ou insira o seu
4. Clique em "Criar Instância"

### Conectar WhatsApp

1. Clique em "Conectar" na instância desejada
2. Escaneie o QR Code com seu WhatsApp
3. Aguarde a conexão ser estabelecida

## 📡 API Evolution - Endpoints

O sistema utiliza os seguintes endpoints da Evolution API:

### Instâncias
- `GET /instance/all` - Listar todas as instâncias
- `POST /instance/create` - Criar nova instância
- `GET /instance/qr` - Obter QR Code
- `GET /instance/status` - Status da instância
- `DELETE /instance/logout` - Desconectar instância
- `POST /instance/disconnect` - Reiniciar instância
- `DELETE /instance/delete/{id}` - Deletar instância
- `POST /instance/connect` - Configurar webhook
- `PUT /instance/{id}/advanced-settings` - Configurações avançadas

### Envio de Mensagens
- `POST /send/text` - Enviar texto
- `POST /send/media` - Enviar mídia (imagem, vídeo, áudio, documento)
- `POST /send/location` - Enviar localização


## 🎨 Temas e Personalização

O projeto suporta tema claro e escuro automaticamente, com gradientes personalizados:

- **Primary:** Gradiente azul/roxo
- **Success:** Gradiente verde
- **Danger:** Gradiente vermelho
- **Info:** Gradiente azul claro
- **Warning:** Gradiente amarelo/laranja

## 🔐 Segurança

- Tokens são mascarados por padrão
- API Keys armazenadas localmente (localStorage)
- Confirmação para ações destrutivas (deletar, desconectar)
- Validação de formulários com Zod

## 📱 Responsividade

Interface totalmente responsiva, otimizada para:
- Desktop (1920px+)
- Laptop (1024px+)
- Tablet (768px+)
- Mobile (320px+)

## 📄 Licença

Este projeto está sob a licença MIT.

---

### Contato
- 📧 Email: contato@packtypebot.com.br
- 🤝 Grupo WhatsApp: [EvoGO](https://chat.whatsapp.com/IJZx0o89kKXFrQCcp8Nvu1)
- 🎥 Nosso Canal: [Youtube](https://www.youtube.com/@packtypebot)

---

### Contribua:
- 🙌  Evolution API : [Crowdfunding](https://contribute.evolution-api.io/)

**Desenvolvido com ❤️ por Pack Typebot.**
