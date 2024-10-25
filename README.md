# Cursor AI Editor Demo from Tripla FE Team

## introduction

Cursor is a modern code editor that is designed to be more efficient and productive. It is built on the same technology as VSCode, but with a focus on providing a more seamless and intuitive coding experience.About Cursor AI editor, after few weeks of reviewing, my conclusion is it provides way more helpful features to FE engineers than github co-pilot:
1. It provides better LLM options,  Claude 3.5 sonnet is way better than ChatGPT about coding, there might be other better options in the future so I think Cursor (3rd party tool) is better than github co-pilot (partner with openAI)
2. It provides full section replacement feature which is far better for daily development than VSCode's autocomplete, VSCode might need extra time to catch up.
3. Cursor can let AI handles multiple files in the same time and it's crazy useful when we want AI edit one file but follow another file's rule, VSCode might need extra time to catch up also.

2 and 3 increase the usefulness of AI from 2% to 15% (base on lines it helped), so I think I'm very sure it's a useful tool.

I recommend we cover its subscription fee by company expense :pray: from FE's perspective.

After we push this tool to All FE engineers, I'm very confident that we already could reduce points for certain type of tasks.

## demo

### case 1

#### better autocomplete than VSCode
1. open `pages/case1.vue`
2. move cursor to end of `fruits`
3. try add watermelon by typing `w`, it should autocomplete
4. there better part is, it will also fix previous line by adding `,`, this is because Cursor able to replace whole section instead only ongoing line.

### case 2

#### fix with command K
1. open `.env`
2. paste following to `.env`
```
VITE_IDENTITY_URL=https://idp.local.tripla.ai
VITE_IDENTITY_KEY=test-xxxx-zzzz-9269-a628de3062e2
VITE_IDENTITY_SECRET=test-yyyy-zzzz-b5b9-8169924e57ac
```
3. select all text and press `command + k`
4. select `fix with command K`, tell it `I want NUXT`
5. accept and done

#### fix with autocomplete
1. open `.env.production`
2. paste following to `.env.production`
```
VITE_IDENTITY_URL=https://idp.tripla.ai
VITE_IDENTITY_KEY=live-2222-4444-9269-a628de3062e2
VITE_IDENTITY_SECRET=live-3333-4444-b5b9-8169924e57ac
```
3. move cursor to end of `VITE_IDENTITY_URL` line
4. wait autocomplete popup, it should fix all three lines with `NUXT_` prefix
5. accept and done

### case 3 

#### Composer, for LLM and future development experience
1. open Composer by `command + i`
2. press `@prompts` and choose `guideline1` to attach to Composer
3. press `@` and attach `pages/case1.vue` to Composer
4. ask it fix `pages/case1.vue`
5. accept and done

# Nuxt Minimal Starter

Look at the [Nuxt documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Setup

Make sure to install dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm dev

# yarn
yarn dev

# bun
bun run dev
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm build

# yarn
yarn build

# bun
bun run build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm preview

# yarn
yarn preview

# bun
bun run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.


