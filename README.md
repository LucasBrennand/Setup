# 🧪 Projeto Vite + Vue + SCSS + TailwindCSS

## 🚀 Iniciando o projeto com Vite e Vue

```bash
npm create vite@latest my-vue-app -- --template vue
cd my-vue-app
npm install
npm run dev
```

---

## 🎨 Configuração do SCSS

1. Crie um arquivo chamado `style.scss`.
2. Instale a extensão **Live Sass Compiler** no VSCode.
3. Clique em **"Watch Sass"** para compilar SCSS automaticamente.
4. Importe o CSS compilado nos seus arquivos:
   ```js
   import './style.css'
   ```

---

## 💨 Configuração do Tailwind CSS

### Instalação
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

### Configuração do Vite

No arquivo `vite.config.ts` ou `vite.config.js`:
```ts
import { defineConfig } from 'vite'
import vue from '@vitejs/plugin-vue'
import tailwindcss from 'tailwindcss'

export default defineConfig({
  plugins: [vue()],
  css: {
    postcss: {
      plugins: [tailwindcss()]
    }
  }
})
```

### CSS Base

No seu arquivo CSS (ex: `style.css`):
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---

✅ Agora você está pronto para desenvolver com **Vite**, **Vue 3**, **SCSS** e **TailwindCSS**!
