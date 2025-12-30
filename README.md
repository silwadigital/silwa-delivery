# Silwa Tecnologia - Plataforma SaaS White-Label

Este projeto é um protótipo de arquitetura de software para uma plataforma SaaS de Delivery Multi-tenant (estilo iFood/Cardápio Digital), desenvolvido com React, TypeScript e Vite.

## 🚀 Ambientes Disponíveis

O sistema possui 4 interfaces integradas:
1.  **Landing Page:** Institucional.
2.  **Gestor (KDS):** Para restaurantes (com IA Gemini).
3.  **App Consumidor:** Cardápio digital.
4.  **Parceiros:** Dashboard de afiliados.

## 📦 Instalação e Execução Local

Você precisará do Node.js instalado.

1.  Clone o repositório.
2.  Instale as dependências:
    ```bash
    npm install
    ```
3.  Rode o servidor de desenvolvimento:
    ```bash
    npm run dev
    ```
4.  Acesse `http://localhost:3000`.

## ☁️ Como Publicar (Deploy)

A maneira mais fácil de visualizar este projeto online é usar a **Vercel**:

1.  Suba este código para o seu GitHub.
2.  Crie uma conta na [Vercel](https://vercel.com).
3.  Clique em **"Add New Project"** e importe seu repositório.
4.  A Vercel detectará automaticamente a configuração do Vite. Clique em **Deploy**.

### Configuração da API Key (IA)

Para que a inteligência artificial (Gemini) funcione no ambiente online:

1.  No painel da Vercel, vá em **Settings > Environment Variables**.
2.  Adicione uma nova variável:
    *   **Key:** `API_KEY`
    *   **Value:** Sua chave da API do Google Gemini.
3.  Redeploy o projeto.

---

**Tecnologias:** React 18, Vite, Tailwind CSS, Google GenAI SDK, Recharts.
