<h1 align="center">VYTA Store</h1>
<p align="center">Headless e-commerce with server-side rendering on Cloudflare and Yampi checkout</p>

<p align="center">
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" /> <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=white" alt="React" /> <img src="https://img.shields.io/badge/TanStack-FF4154?style=flat-square&logo=reactquery&logoColor=white" alt="TanStack" /> <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare" /> <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
</p>

<p align="center">
<a href="https://vytacore.com.br"><b>Live store</b></a>
</p>

<p align="center"><img src="loja-home.png" width="900" alt="VYTA store home page" /></p>

> **Note:** the source code is private (production systems). This repository is a technical overview: what it does, how it is built and what it looks like. Happy to walk through the code in an interview — reach me on [LinkedIn](https://www.linkedin.com/in/guilherme-vytacore/).

## Overview

The brand's official online store, live at [vytacore.com.br](https://vytacore.com.br). The storefront is custom-built with server-side rendering; catalog, inventory and checkout come from Yampi through its API.

## Highlights

- **SSR with TanStack Start**, deployed to Cloudflare (Workers/Pages via Nitro)
- **Yampi API integration**: products, SKUs, inventory, coupons, free-shipping rules, product reviews and webhooks
- **Bundles and kits** assembled in the store with native checkout
- **Split orders across suppliers**, each with its own shipping label
- **Partner portal** integrated with Tiny ERP, with access rules enforced server-side
- **Order tracking** linked to the customer area
- **40+ test and probe scripts** covering the storefront, cart and purchase flows

## Architecture

```mermaid
flowchart LR
  U["Shopper"] --> SF["Storefront<br/>TanStack Start (SSR)"]
  SF --> CF["Cloudflare Workers"]
  CF <--> YAMPI["Yampi API<br/>catalog, stock, checkout"]
  CF <--> TINY["Tiny ERP<br/>orders, labels"]
  SF --> CHK["Yampi checkout"]
```

## Tech stack

- **Frontend:** TanStack Start, React 19, TypeScript, Zustand, TanStack Query, Tailwind CSS v4, shadcn/ui
- **Integrations:** Yampi, Tiny ERP
- **Infrastructure:** Cloudflare, Supabase

---

<details>
<summary><b>Versão em português</b></summary>

> **Observação:** o código-fonte é privado (sistemas em produção). Este repositório é uma visão técnica do projeto. Posso apresentar o código em uma entrevista — fale comigo pelo [LinkedIn](https://www.linkedin.com/in/guilherme-vytacore/).

## Visão geral

Loja oficial da marca, no ar em [vytacore.com.br](https://vytacore.com.br). O front é próprio, com renderização no servidor; catálogo, estoque e checkout vêm da Yampi pela API.

## Destaques

- **SSR com TanStack Start** publicado no Cloudflare
- **Integração com a API da Yampi**: produtos, SKUs, estoque, cupons, frete grátis, comentários e webhooks
- **Kits e combos** com checkout nativo
- **Pedidos divididos entre fornecedores**, com etiquetas separadas
- **Portal de parceiro** integrado ao ERP Tiny
- **Rastreio de pedidos** na área do cliente
- **40+ scripts de teste** da vitrine e dos fluxos de compra

## Stack

- **Frontend:** TanStack Start, React 19, TypeScript, Zustand, TanStack Query, Tailwind CSS v4, shadcn/ui
- **Integrações:** Yampi, Tiny ERP
- **Infra:** Cloudflare, Supabase

</details>
