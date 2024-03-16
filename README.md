This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
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

## Commands I used for configuration of CI/CD in this project.

npm install --save-dev prettier eslint-config-prettier eslint-plugin-prettier

npm install --save-dev husky lint-staged

git init
npx husky install
npx husky add .husky/pre-commit "npx lint-staged"

npm install --save-dev @commitlint/{cli,config-conventional}

npx husky add .husky/commit-msg 'npx --no-install commitlint --edit "$1"'  Now create commitlint.config.cjs

// adding this will create static site for next.js 14 for GitHub pages const nextConfig = { output: 'export’}
