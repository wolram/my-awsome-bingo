# Copilot Instructions — My Awsome Bingo

## Development Checklist
- [ ] `npm run lint` passes
- [ ] `npm run build` succeeds
- [ ] `npm test` passes (especially `bingoLogic` tests)

## Quick Reference

**Big Picture**: Frontend-only React + Vite app (no backend). Static deploy to GitHub Pages via push to `main`.

**Key Files**
- Logic: `src/utils/bingoLogic.ts` + tests
- State: `src/hooks/useBingoGame.ts`
- Components: `src/components/` (Board, Square, Screens)
- Content: `src/data/questions.ts`

**Scripts**
- `npm install` (Node 22+)
- `npm run dev` → http://localhost:5173/
- `npm test` (Vitest)
- `npm run lint` (ESLint)
- `npm run build` (TypeScript + Vite)

**Conventions**
- Board: 25 squares (IDs 0–24), center (index 12) = free space (marked by default)
- `toggleSquare()` returns new immutable array
- Win detection: rows/columns/diagonals via `checkBingo()`
- Add questions via `src/data/questions.ts`

**Before Opening PR**
- Run full checklist above
- Manual test: start game → mark squares → detect bingo
- For logic changes: update `src/utils/bingoLogic.test.ts`

**Design & Styling**
- Tailwind v4: see `.github/instructions/tailwind-4.instructions.md`
- Frontend design: see `.github/instructions/frontend-design.instructions.md`

**Key Gotchas**
- Board size (24 + 1 free) is hardcoded in all win-check functions
- No backend: external integrations must be documented in README
