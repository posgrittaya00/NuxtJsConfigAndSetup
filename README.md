# Setup the project
 Open a terminal (if you're using Visual Studio Code, you can open an integrated terminal) and use the following command to create a new starter project:

|   |command
| ------------ |
|  npx | `npx nuxi@latest init <project-name>`|
| pnpm  |`pnpm dlx nuxi@latest init <project-name>`|
|bun   |`bunx nuxi@latest init <project-name>`|

## Development Server
Now you'll be able to start your Nuxt app in development mode:

|   |command
| ------------ |
|yarn |  yarn dev --open |
|npm|  npm run dev -- -o |
|pnpm| pnpm dev -o  |
|bun|bun run dev -o|

#Nuxt Tailwind
1.Install @nuxtjs/tailwindcss dependency to your project:

|   |  command |
| ------------ | ------------ |
|  nuxi | npx nuxi@latest module add tailwindcss  |
|   yarn|   yarn add -D @nuxtjs/tailwindcss|
|   npm|   npm install -D @nuxtjs/tailwindcss|
|pnpm | pnpm i -D @nuxtjs/tailwindcss|

> nuxt.config2. If not already done, add it to your modules section in your nuxt.config:

```ts
export default defineNuxtConfig({
  modules: ['@nuxtjs/tailwindcss']
})

```

#Primevue 
- ##**Download **
> PrimeVue is available for download on npm registry. For this setup, we'll also use the primevue-nuxt module.

##### npm
```ts
npm install primevue
npm install --save-dev nuxt-primevue```
#####yarn
```ts
yarn add primevue
yarn add --dev nuxt-primevue```
#####  pnpm
```ts
pnpm add primevue
pnpm add -D nuxt-primevue```

- ##**Nuxt Config**
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

- ##**Preset**
> Download a release from github, alternatively you may use Preset Builder to dynamically build your release file with the components you need as the pre-build release package contains all the available components. Once the zip is downloaded, extract the contents to a folder of your choice e.g. ./presets and then in your nuxt-config file, configure the importPT property of PrimeVue to the main preset file.


