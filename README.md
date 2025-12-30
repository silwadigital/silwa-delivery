# Silwa Tecnologia - Plataforma SaaS White-Label

Este projeto é um protótipo de arquitetura de software para uma plataforma SaaS de Delivery Multi-tenant (estilo iFood/Cardápio Digital), focada em alta performance e escalabilidade.

O sistema demonstra a separação de responsabilidades entre diferentes "personas" da aplicação: Consumidor Final, Restaurante, Parceiro (Afiliado) e Landing Page Institucional.

## 🚀 Funcionalidades Demonstradas

O projeto está dividido em 4 interfaces lógicas dentro de uma SPA (Single Page Application):

1.  **Institucional (Landing Page):** Página de alta conversão para atrair novos restaurantes e parceiros.
2.  **Gestor de Pedidos (KDS):** Dashboard para o restaurante gerenciar pedidos em tempo real (Pendente -> Preparo -> Entrega).
    *   *Feature IA:* Geração de descrições de pratos usando **Google Gemini**.
3.  **App do Consumidor:** Interface mobile-first para realização de pedidos (Cardápio Digital).
4.  **Portal do Parceiro:** Sistema de afiliados com dashboard de comissões e insights de crescimento gerados por IA.

## 🛠️ Tecnologias Utilizadas

*   **Frontend:** React 19
*   **Estilização:** Tailwind CSS (via CDN)
*   **Ícones:** Lucide React
*   **Gráficos:** Recharts
*   **Inteligência Artificial:** Google GenAI SDK (Gemini 2.5/3.0)
*   **Buildless:** Utiliza ES Modules via `esm.sh`, permitindo execução sem `npm install` complexos para prototipagem rápida.

## 📦 Como Rodar

Como este projeto utiliza uma arquitetura moderna baseada em ES Modules via browser:

1.  Clone este repositório.
2.  Você precisa de um servidor HTTP simples (não abra o arquivo `index.html` direto clicando duas vezes, pois o CORS bloqueará os módulos).
3.  Se tiver o VS Code instalado, use a extensão **Live Server**.
4.  Ou via terminal com Python:
    ```bash
    python3 -m http.server
    ```
5.  Acesse `http://localhost:8000`.

## 🔑 Configuração da API (Gemini)

Para que as funcionalidades de IA (descrição de pratos e insights de parceiros) funcionem, você precisa de uma API Key do Google Gemini.

**Nota de Segurança:** Nunca faça commit da sua chave de API diretamente no GitHub.
Em um ambiente de produção (Vite/Next.js), isso seria configurado via arquivos `.env`.

## 📝 Estrutura de Arquivos

*   `index.html`: Ponto de entrada e import maps.
*   `App.tsx`: Roteamento simples entre as visões.
*   `components/`: Componentes visuais das 4 aplicações.
*   `services/`: Integração com serviços externos (Gemini AI).
*   `types.ts`: Definições de tipos TypeScript compartilhados.

---

Desenvolvido como demonstração de arquitetura SaaS.
