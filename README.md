# Instadraw

Share your drawings with the world with this [Nuxt application](https://nuxt.com) using [NuxtHub Blob storage](https://hub.nuxt.com/docs/storage/blob) (Cloudflare R2) and deployed on the Edge (Cloudflare Pages).

- [Demo](https://draw.nuxt.dev)
- [NuxtHub docs](https://hub.nuxt.com)
- [Nuxt docs](https://nuxt.com)

## Features

- Image upload with [`useUpload()`](https://hub.nuxt.com/docs/storage/blob)
- Auth with Google & GitHub based on [`nuxt-auth-utils`](https://github.com/Atinux/nuxt-auth-utils)
- Draw with [`signature_pad`](https://github.com/szimek/signature_pad)

## Setup

Make sure to install the dependencies:

```bash
pnpm install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
pnpm dev
```

## Production

Build the application for production:

```bash
pnpm build
```

## Environment Variables

Copy the `.env.example` file to `.env` and fill in the required environment variables:

```bash
cp .env.example .env
```

You may want to create Google and GitHub OAuth applications.

## Deploy on the Edge

Deploy the application on the Edge with [NuxtHub](https://hub.nuxt.com):

```bash
npx nuxthub deploy
```

Then manage the drawings of your users in the [NuxtHub Admin](https://admin.hub.nuxt.com).

You can also deploy using [Cloudflare Pages CI](https://hub.nuxt.com/docs/getting-started/deploy#cloudflare-pages-ci).
