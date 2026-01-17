# Next.js + Vercel baseline

Denna playbook beskriver Mats standardsetup för nya Next.js-projekt.

## Grundprinciper
- Börja med `npx create-next-app@latest --ts`
- Push:a initial commit direkt till GitHub
- Koppla repo till Vercel samma dag
- Använd Neon (Vercel Postgres) för datalager

## Steg-för-steg
1. Skapa repo på GitHub och klona lokalt
2. Kör create-next-app med App Router och Tailwind
3. Lägg till `.env.example` med `DATABASE_URL` och övriga variabler
4. Initiera Prisma om databas behövs
5. Skapa Neon-projekt och koppla till Vercel med "Connect"-knappen
6. Sätt upp Vercel Project → importera från GitHub → root = `/`
7. Verifiera `npm run lint` och `npm run test` (om finns)
8. Deploy preview → gör smoke test innan merge

## Viktiga regler
- Inga hemligheter i repo
- All konfiguration dokumenteras i Memory Vault
- Boris-komponenter ska vara enkla att aktivera per projekt
