
## Create Project

Open a terminal (if you’re using Visual Studio Code, you can open an integrated terminal) and use the following command to create a new starter project:
- **npx**	

```bash
  npx nuxi@latest init <project-name>
```

- **pnpm**	

```bash
  pnpm dlx nuxi@latest init <project-name>
```

- **bun**

```bash
  bunx nuxi@latest init <project-name>
```

## Development
Install @nuxtjs/tailwindcss dependency to your project:
- **yarn**
```bash
yarn dev —open
```
- **npm**
```bash
npm run dev — -o
```
- **pnpm**
```bash
pnpm dev -o
```
- **bun**
```bash
bun run dev -o
```

> nuxt.config2. If not already done, add it to your modules section in your nuxt.config:
```ts
export default defineNuxtConfig({
  modules: ['@nuxtjs/tailwindcss']
})

```