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

![image](https://github.com/vaibhavmalhotra002/Nextjs14cicd/assets/76607940/b71e89cf-f33e-4e3e-86fe-bf03d6cf87d5)


git init  (initalize git repository)

npx husky-init && npm install
npm install husky --save-dev
npx husky install


npx husky add .husky/pre-commit "npx lint-staged"

npm install --save-dev @commitlint/{cli,config-conventional} (To keep a check & apply rules for commit messages)

npx husky add .husky/commit-msg 'npx --no-install commitlint --edit "$1"' 

Now create commitlint.config.cjs for applying rules for writing commit messages
<img width="1440" alt="Screenshot 2024-03-16 at 3 33 33 PM" src="https://github.com/vaibhavmalhotra002/Nextjs14cicd/assets/76607940/9c87bd51-a954-4916-8f9a-0e359f6eb1f6">


// adding this will create static site for next.js 14 for GitHub pages const nextConfig = { output: 'export’}
