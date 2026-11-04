# Portal Comercial Senac Tecnologia — React + Vite

Projeto React profissional, responsivo, com busca, filtros e cards que abrem **os quatro sites originais** com as grades curriculares integradas.

## Requisitos
- Node.js 20.19+ ou 22.12+ (recomendado Node.js 22)
- VS Code

## Executar localmente
```bash
npm install
npm run dev
```
Abra o endereço mostrado no terminal (normalmente http://localhost:5173).

## Validar o build de produção
```bash
npm run build
npm run preview
```

## Deploy Vercel
1. Publique esta pasta em um repositório GitHub.
2. Em https://vercel.com/new, importe o repositório.
3. Framework: **Vite**. Build: `npm run build`. Output: `dist`.
4. Clique em Deploy.

Alternativa pelo terminal:
```bash
npx vercel
npx vercel --prod
```

## Estrutura
- `src/`: portal React (cards, filtros, explicações, FAQ).
- `public/cursos/`: sites HTML/CSS originais de cada curso, com grades integradas. São copiados integralmente para `dist/cursos/` pelo Vite.
- `vercel.json`: configurações de build.

**Importante:** Não abra o `index.html` diretamente dentro do ZIP. Extraia o projeto e use `npm run dev`. As páginas de cursos são arquivos estáticos preservados dos materiais originais, acessíveis pelo React via links diretos. O portal principal é React; as páginas originais continuam HTML para preservar o conteúdo e o design existente.

**Matrizes:** confira informações curriculares e pré-requisitos com a unidade antes de utilizá-las em matrículas.
