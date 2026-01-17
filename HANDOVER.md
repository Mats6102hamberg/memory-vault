# Memory Vault - Handover

## Repository
- **GitHub:** https://github.com/Mats6102hamberg/memory-vault
- **Branch:** main
- **Structure:** Root repo med markdown docs + Next.js frontend i `frontend/`

## Local Setup

```bash
# Clone
git clone https://github.com/Mats6102hamberg/memory-vault.git
cd memory-vault

# Install frontend dependencies
cd frontend
npm install

# Run dev server
npm run dev
# → http://localhost:3000
```

## Deploy (Vercel)

**VIKTIGT:** Root Directory = `frontend/`

```bash
# Vercel CLI
cd memory-vault
vercel

# Eller via Vercel Dashboard:
# 1. Import GitHub repo: Mats6102hamberg/memory-vault
# 2. Framework Preset: Next.js
# 3. Root Directory: frontend/
# 4. Build Command: next build (default)
# 5. Output Directory: (lämna tom)
```

## Git Workflow

```bash
# Alltid från root
cd ~/CascadeProjects/memory-vault

# Kontrollera status
git status

# Lägg till ändringar
git add .
git commit -m "beskrivning"

# Push
git push origin main

# VIKTIGT: Inga nested repos!
find . -name ".git" -type d -maxdepth 4
# Ska ENDAST visa: ./.git
```

## Kritiska Filer

### Markdown Docs
- `start-here/START.md` - Huvudindex
- `start-here/HOW_TO_USE_THIS.md` - Workflow
- `projects/*/NOW.md` - Projektstatus
- `playbooks/*.md` - Standardprocedurer
- `brand/*.md` - Brand guidelines

### Frontend
- `frontend/src/app/docs/[...slug]/page.tsx` - Dynamisk markdown rendering
- `frontend/src/lib/docs-map.ts` - Route mapping och navigation
- `frontend/src/lib/get-markdown.ts` - Markdown file reader
- `frontend/src/components/sidebar.tsx` - Navigation sidebar

## Felsökning

### "Repository not found" vid push
```bash
git remote -v  # Kontrollera URL
git remote remove origin
git remote add origin https://github.com/Mats6102hamberg/memory-vault.git
git push -u origin main
```

### Nested repo upptäckt
```bash
rm -rf frontend/.git
git add .
git commit -m "Fix nested repo"
git push
```

### Vercel hittar inte Next.js
- Kontrollera Root Directory = `frontend/` i Vercel settings
- Verifiera att `frontend/package.json` finns

## Dependencies

### Frontend
- Next.js 15+
- React 19+
- TypeScript
- Tailwind CSS
- react-markdown
- remark-gfm

## Environment Variables
Inga secrets i detta repo. Allt är public documentation.

## Kontakt
Mats Hamberg - GitHub: @Mats6102hamberg
