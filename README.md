# Full-Stack-E-Commerce-Dashboard-CMS

Next.js@13 App-Router, React, Tailwind, Prisma, MySQL

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm i
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Environment Variable

[Clerk Authentication system integrate](https://clerk.com/docs/references/nextjs/)

```bash
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=<key>
CLERK_SECRET_KEY=<secret key>
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/
```

[Cloudenery](https://cloudinary.com/documentation/react_image_and_video_upload)

```bash
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=<namekey>
```

## [Prisma Setup with mysql](https://www.prisma.io/docs/concepts/database-connectors/mysql)

```bash
npm install @prisma/client prisma
# or
yarn add @prisma/client prisma

npx prisma init --datasource-provider mysql


#Update your .env prisma generated mysql connection link then write your model into the schema.prisma file after that run this below cli command
npx prisma generate
# or
yarn prisma generate

npx prisma db push
```

## [Environment Variable for prisma mysql](https://www.prisma.io/docs/getting-started/setup-prisma/start-from-scratch/relational-databases/connect-your-database-node-mysql)

```bash
DATABASE_URL="mysql://<user>:<password>@127.0.0.1:3306/<db_name>?KEY1=VALUE&KEY2=VALUE&KEY3=VALUE"
```
