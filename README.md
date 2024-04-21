
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


## Tailwind
  Install @nuxtjs/tailwindcss dependency to your project:
|   |  command |
| ------------ | ------------ |
|  nuxi | npx nuxi@latest module add tailwindcss  |
|   yarn|   yarn add -D @nuxtjs/tailwindcss|
|   npm|   npm install -D @nuxtjs/tailwindcss|
|pnpm | pnpm i -D @nuxtjs/tailwindcss|

> nuxt.config. If not already done, add it to your modules section in your nuxt.config:

```ts
export default defineNuxtConfig({
  modules: ['@nuxtjs/tailwindcss']
})
```

## Primevue 
**- Download**
> PrimeVue is available for download on npm registry. For this setup, we'll also use the primevue-nuxt module.

### npm
```ts
npm install primevue
npm install --save-dev nuxt-primevue
```
### yarn
```ts
yarn add primevue
yarn add --dev nuxt-primevue
```
### pnpm
```ts
pnpm add primevue
pnpm add -D nuxt-primevue
```

**- Nuxt Config**
> In your nuxt-config file, add the nuxt-primevue module and configure PrimeVue to be unstyled.

```ts
export default defineNuxtConfig({
    modules: [
        'nuxt-primevue'
    ],
    primevue: {
        options: {
          unstyled: true
        },
    }
})

```
