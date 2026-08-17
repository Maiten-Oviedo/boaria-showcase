# Boaria Systems — Catálogos SaaS para PyMEs

> Repositorio de showcase. El código fuente del producto es privado (SaaS comercial con cliente pagante).

<img width="1915" height="965" alt="image" src="https://github.com/user-attachments/assets/5589c4e1-c358-4d7c-ad90-29dc6600e3bc" />

## Qué es Boaria

**Boaria Systems** es un SaaS que transforma listas de precios en Excel o Google Sheets en catálogos web completos para PyMEs, sin que el comercio tenga que aprender ninguna herramienta técnica. El cliente sigue actualizando precios en su planilla como siempre — el catálogo web se sincroniza automáticamente.

Fundé Boaria en abril 2025. Cliente activo pagante desde marzo 2026.

## Cliente en producción

🌐 **Apple Store Mendoza** — [apple-store-mendoza.vercel.app](https://apple-store-mendoza.vercel.app)

Comercio de productos Apple (iPhone, MacBook, accesorios) en Mendoza, Argentina. Sitio activo, en producción, sirviendo tráfico real todas las semanas.

## Features

- 🔄 **Sync automática con Google Sheets** — el comercio actualiza precios en su planilla y el sitio se refleja solo, sin intervención manual.
- 💵 **Conversión automática de dólar** vía API en tiempo real.
- 🛒 **Carrito integrado** con persistencia y flujo de checkout.
- 💬 **Consultas directas por WhatsApp** — cada producto tiene su CTA a chat con el comercio.
- 🏢 **Arquitectura multi-tenant** — onboarding rápido de nuevos comercios sin código nuevo.

## Modelo de negocio

- SaaS a USD 9/mes por cliente.
- Onboarding en menos de un día (sync con la planilla del cliente + configuración de branding).

## Stack

- **Framework:** Astro
- **Frontend:** React + TypeScript
- **Estilos:** TailwindCSS
- **Backend:** Node.js
- **Base de datos:** PostgreSQL
- **APIs externas:** Google Sheets API, conversión de dólar (API pública)
- **Deploy:** Vercel

## Arquitectura (resumen)

```
Cliente (Astro + React) 
   ↓ 
API Node.js (multi-tenant routing)
   ↓
├── PostgreSQL (metadata: tenants, config, branding)
├── Google Sheets API (source of truth para catálogos)
└── API dólar (cotización en tiempo real)
```

## Screenshots

**Hero**
<img width="1908" height="959" alt="image" src="https://github.com/user-attachments/assets/b0bfa84c-afdc-4b34-9c2e-b8ad805dfaf5" />
**Listado de productos**
<img width="1909" height="938" alt="image" src="https://github.com/user-attachments/assets/6272ac5b-a341-451f-a6b3-f1d6de3c6226" />
**Ficha de producto**
<img width="1910" height="938" alt="image" src="https://github.com/user-attachments/assets/94aad0a3-bb9b-4090-a0ee-dee4f3d5bfb6" />
**Carrito**
<img width="1910" height="962" alt="image" src="https://github.com/user-attachments/assets/c444a96b-a112-4271-a62b-1ba912403438" />

## Contacto

- Sitio en producción: [apple-store-mendoza.vercel.app](https://apple-store-mendoza.vercel.app)
- Portfolio del desarrollador: [maitendev.vercel.app](https://maitendev.vercel.app)
- Email: [maitenoviedo513@gmail.com](mailto:maitenoviedo513@gmail.com)
- LinkedIn: [linkedin.com/in/maiten-oviedo](https://linkedin.com/in/maiten-oviedo)
