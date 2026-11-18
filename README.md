<h1 align="center">🛒 Ecommerce oficial da marca VytaCore com joint venture com a marca Nação Verde</h1>
<p align="center"><b>E-commerce headless com SSR no Cloudflare e checkout Yampi</b></p>

<p align="center">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" /> <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=white" /> <img src="https://img.shields.io/badge/TanStack-FF4154?style=for-the-badge&logo=reactquery&logoColor=white" /> <img src="https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" /> <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
</p>

>  O código-fonte deste projeto é **privado**. Este repositório é uma vitrine com a visão geral, a arquitetura e a stack. Quer saber mais? Fale comigo pelo [LinkedIn](https://www.linkedin.com/in/luiz-guilherme-dos-santos-820a792a4/).

##  O que é

A loja oficial da marca, no ar em [vytacore.com.br](https://vytacore.com.br). O front é próprio, com renderização no servidor, e o catálogo, o estoque e o checkout vêm da Yampi pela API.

##  Destaques

-  **SSR com TanStack Start**, publicado no Cloudflare (Workers/Pages via Nitro)
-  **Integração com a API da Yampi**: produtos, SKUs, estoque, cupons, frete grátis, comentários e webhooks
-  **Kits e combos** montados na loja, com checkout nativo
-  **Pedidos divididos entre fornecedores**, com etiquetas separadas
-  **Portal de parceiro** integrado ao ERP Tiny, com regras de acesso aplicadas no servidor
-  **Rastreio de pedidos** integrado à área do cliente
-  **40+ scripts de teste** para a vitrine, o carrinho e os fluxos de compra

##  Stack

- **Frontend:** TanStack Start · React 19 · TypeScript · Zustand · TanStack Query · Tailwind CSS v4 · shadcn/ui
- **Integrações:** Yampi · Tiny ERP
- **Infra:** Cloudflare · Supabase
