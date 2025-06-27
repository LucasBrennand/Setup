# 🧪 Projeto Vite + React + SCSS + TailwindCSS

## 🚀 Iniciando o projeto com Vite e React

```bash
npm create vite@latest my-react-app -- --template react
cd my-react-app
npm install
npm run dev
```

---

## 🎨 Configuração do SCSS

1. Crie um arquivo chamado `style.scss`.
2. Rode esse comando no terminal
```bash
npm install -D sass-embedded
```
3. Importe o SCSS nos seus arquivos:
   ```jsx
   import './style.scss'
   ```

---

## 💨 Configuração do Tailwind CSS

### Instalação
```bash
npm install tailwindcss @tailwindcss/vite
```

### Configuração do Vite

No arquivo `vite.config.ts` ou `vite.config.js`:
```ts
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [react(), tailwindcss()],
})
```

### CSS Base

No seu arquivo CSS (ex: `style.css`):
```css
@import "tailwindcss";
```

---

✅ Agora você está pronto para desenvolver com **Vite**, **react 3**, **SCSS** e **TailwindCSS**!
