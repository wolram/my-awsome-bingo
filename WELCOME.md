# Welcome — My Awsome Bingo

Bem-vindo! Este repositório contém um jogo de Bingo social (frontend-only).

Quick start

```bash
npm install
npm run dev
```

- Abra: http://localhost:5173/
- Testes: `npm test` (Vitest) — a lógica de bingo tem cobertura em `src/utils/bingoLogic.test.ts`.
- Estrutura útil: `src/components/`, `src/hooks/useBingoGame.ts`, `src/data/questions.ts`.

Dicas rápidas

- A grade tem 25 quadrados; o centro (índice 12) é um espaço grátis.
- Preserve imutabilidade ao alterar o estado (ex.: `toggleSquare`).
- Siga `.github/instructions/tailwind-4.instructions.md` ao alterar estilos.

Quer que eu adicione este tour ao `.lab/GUIDE.md` também? (responda sim/não)
