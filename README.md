<div align="center">

# Bela Via Fashion

**Base de e-commerce de moda construída com React, Vite e shadcn/ui**

[![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-5-646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-3-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000000?logo=shadcnui&logoColor=white)](https://ui.shadcn.com/)
[![Licença: MIT](https://img.shields.io/badge/licen%C3%A7a-MIT-blue.svg)](./LICENSE)

</div>

---

## 📖 Sobre

O **Bela Via Fashion** é um projeto de vitrine/loja de moda para a web. O objetivo do domínio é oferecer um e-commerce de vestuário com identidade visual própria, navegação entre produtos e um sistema de design consistente — atendendo a consumidores que buscam peças de moda em uma experiência de compra moderna e responsiva.

O projeto entrega uma **base sólida de design system** pronta para crescer: tokens de cor em HSL (tema claro e escuro), a biblioteca completa de componentes **shadcn/ui**, roteamento e layout responsivo. A página inicial funciona como **vitrine viva** desse sistema de design — [veja ao vivo](https://bela-via-fashion.vercel.app).

A base foi montada para acelerar a interface do e-commerce, fornecendo componentes de UI prontos (formulários, diálogos, tabelas, abas, carrosséis, gráficos, notificações e mais) e integração preparada com gerenciamento de estado assíncrono, de modo que o foco fique na regra de negócio da moda.

**Próximos passos:** fluxos de catálogo, carrinho e checkout.

## ✨ Funcionalidades

- **Sistema de design** com variáveis CSS em HSL e suporte a **tema claro e escuro** (`darkMode: ["class"]`, definidas em `src/index.css`).
- **Biblioteca completa de componentes shadcn/ui** em `src/components/ui` (accordion, alert, avatar, badge, breadcrumb, button, calendar, card, carousel, chart, checkbox, command, dialog, drawer, dropdown-menu, form, input, menu de navegação, paginação, popover, progress, select, sheet, sidebar, skeleton, slider, switch, table, tabs, toast, tooltip, entre outros).
- **Roteamento com React Router** e rota curinga (`*`) que direciona para a página **NotFound**.
- **Provisionamento global** de `QueryClientProvider` (TanStack React Query), `TooltipProvider` e dois sistemas de notificação (`Toaster` e `Sonner`) em `src/App.tsx`.
- **Utilitário `cn`** (`src/lib/utils.ts`) para composição de classes com `clsx` e `tailwind-merge`.
- **Hooks utilitários** `use-mobile` (detecção de viewport) e `use-toast`.
- **Ferramentas de formulário e validação** disponíveis no projeto (React Hook Form, `@hookform/resolvers` e Zod) e **gráficos** com Recharts.

## 🛠️ Tecnologias

<p>
<img src="https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white" alt="React" />
<img src="https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white" alt="TypeScript" />
<img src="https://img.shields.io/badge/Vite-5-646CFF?logo=vite&logoColor=white" alt="Vite" />
<img src="https://img.shields.io/badge/Tailwind%20CSS-3-06B6D4?logo=tailwindcss&logoColor=white" alt="Tailwind CSS" />
<img src="https://img.shields.io/badge/shadcn%2Fui-000000?logo=shadcnui&logoColor=white" alt="shadcn/ui" />
<img src="https://img.shields.io/badge/React%20Router-6-CA4245?logo=reactrouter&logoColor=white" alt="React Router" />
<img src="https://img.shields.io/badge/TanStack%20Query-5-FF4154?logo=reactquery&logoColor=white" alt="TanStack Query" />
<img src="https://img.shields.io/badge/Zod-3-3E67B1?logo=zod&logoColor=white" alt="Zod" />
</p>

- **React 18** + **TypeScript** + **Vite**
- **shadcn/ui** (componentes baseados em Radix UI) e **Tailwind CSS** + `tailwindcss-animate`
- **React Router DOM**, **TanStack React Query**
- **React Hook Form** + **Zod**, **Recharts**
- **lucide-react** (ícones), **sonner** e **vaul** (drawer)
- **next-themes** (temas claro/escuro)

## 📁 Estrutura do projeto

```
bela-via-fashion/
├── public/
│   ├── favicon.ico
│   ├── placeholder.svg
│   └── robots.txt
├── src/
│   ├── components/
│   │   ├── ui/                  # Biblioteca de componentes shadcn/ui
│   │   └── NavLink.tsx
│   ├── hooks/
│   │   ├── use-mobile.tsx
│   │   └── use-toast.ts
│   ├── lib/utils.ts             # Utilitário cn (clsx + tailwind-merge)
│   ├── pages/
│   │   ├── Index.tsx            # Página inicial (conteúdo de exemplo)
│   │   └── NotFound.tsx         # Página 404
│   ├── App.tsx                  # Provedores globais e rotas
│   ├── index.css                # Tokens de design (HSL) e tema claro/escuro
│   └── main.tsx
├── index.html
├── components.json              # Configuração do shadcn/ui
├── package.json
├── tailwind.config.ts
├── tsconfig.json
└── vite.config.ts
```

## 🚀 Como rodar localmente

Pré-requisitos: **Node.js** e **npm**.

```bash
# 1. Instalar as dependências
npm install

# 2. Iniciar o servidor de desenvolvimento (http://localhost:8080)
npm run dev
```

Scripts disponíveis:

```bash
npm run dev        # Servidor de desenvolvimento
npm run build      # Build de produção
npm run preview    # Pré-visualização do build
npm run lint       # Análise estática com ESLint
```

## 📄 Licença

Distribuído sob a **Licença MIT**. Veja [`LICENSE`](./LICENSE).
