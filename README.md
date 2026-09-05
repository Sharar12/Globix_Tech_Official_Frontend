# Globix Tech — Frontend

The frontend for the **Globix Tech** company website and digital services platform. It is built with **Astro, TypeScript/JavaScript, Tailwind CSS, and Vercel deployment support**, with interactive and server-side features for company pages, service information, blog content, contact submissions, and an admin area.

## Overview

This repository contains the website frontend only. The current project uses Astro's page-based architecture and separates reusable UI into components, layouts, data, scripts, and styles.

## Tech Stack

| Technology | Purpose |
| --- | --- |
| [Astro](https://astro.build/) 4 | Web framework and page rendering |
| TypeScript / JavaScript | Application logic and typing |
| [Tailwind CSS](https://tailwindcss.com/) 3 | Responsive styling |
| [Astro Sitemap](https://docs.astro.build/en/guides/integrations-guide/sitemap/) | Sitemap generation |
| [Vercel adapter](https://docs.astro.build/en/guides/integrations-guide/vercel/) | Vercel deployment support |
| Poppins | Typography |
| jsPDF / AutoTable | PDF generation |
| SheetJS (`xlsx`) | Spreadsheet generation/processing |
| Sharp | Image processing |
| Resend | Contact/email integration |

The repository targets **Node.js 20.x**.

## Main Website Areas

The current Astro pages include:

- Home
- About
- Services
- Portfolio
- R&D wing
- Contact
- Blog
- Solutions
- Login
- Admin
- Custom 404 page

These routes are represented under `src/pages/`.

## Frontend Capabilities

- Responsive company website and marketing pages
- Reusable Astro components and layouts
- Service and solution presentation
- Portfolio/project presentation
- Blog structure
- Contact form interface
- Login and admin-facing pages
- Client/server scripts for interactive features
- PDF and spreadsheet-related frontend utilities
- SEO-oriented sitemap integration

## Project Structure

```text
Globix_Tech_Official_Frontend/
├── src/
│   ├── assets/             # Source assets
│   ├── components/         # Reusable UI components
│   ├── data/               # Page/content data
│   ├── layouts/            # Shared Astro layouts
│   ├── pages/              # Route/page files
│   │   ├── admin/          # Admin pages
│   │   ├── api/            # API-facing page endpoints
│   │   ├── blog/           # Blog pages
│   │   ├── solutions/      # Solution pages
│   │   ├── about.astro
│   │   ├── contact.astro
│   │   ├── index.astro
│   │   ├── login.astro
│   │   ├── portfolio.astro
│   │   ├── rd-wing.astro
│   │   └── services.astro
│   ├── scripts/            # Client/server scripts
│   └── styles/             # Shared styles
│
├── public/                 # Public static assets
├── astro.config.mjs        # Astro configuration
├── tailwind.config.mjs     # Tailwind configuration
├── env.example             # Environment variable template
├── package.json
└── README.md
```

## Environment Variables

The repository includes an `env.example` file with configuration for administrative access, Resend email delivery, contact email, and Gemini AI functionality.

Example:

```env
ADMIN_PASSWORD=your-secure-password-here
RESEND_API_KEY=
CONTACT_EMAIL=your-contact-email
GEMINI_API_KEY=
```

Do not commit real credentials, API keys, passwords, or private production configuration.

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Sharar12/Globix_Tech_Official_Frontend.git
cd Globix_Tech_Official_Frontend
```

### 2. Install dependencies

With npm:

```bash
npm install
```

Or with pnpm:

```bash
pnpm install
```

### 3. Configure environment variables

Copy `env.example` to your local environment file and populate the required values.

### 4. Start development

```bash
npm run dev
```

Astro starts the development server and prints the local URL in the terminal.

## Available Scripts

```bash
npm run dev       # Start Astro development server
npm run start     # Start Astro development server
npm run build     # Build the production site
npm run preview   # Preview the production build locally
npm run astro     # Run the Astro CLI
```

## Deployment

The project includes the Astro Vercel adapter, so the repository is configured with Vercel deployment support.

For production deployments:

1. Install dependencies.
2. Set production environment variables.
3. Run `npm run build`.
4. Deploy using the configured deployment target.

## Frontend Scope

This repository is the **Globix Tech frontend/web application**. It contains presentation, routing, reusable UI, static assets, frontend scripts, and frontend-related integrations. Any external backend, database, authentication service, or server-side business logic should be treated as a separate concern.

## Security Notes

- Never commit populated environment files containing secrets.
- Replace demo/test data before production releases.
- Keep administrative credentials outside the repository.
- Treat backend/server-side validation as the final security boundary.

## License

This project is distributed under the license included in the repository.

<!-- README refresh: documentation-only change. -->
