# FakturaSnap – Handover

## Repo & deploy
- GitHub: https://github.com/mats-hamberg/fakturasnap (placeholder)
- Production: https://fakturasnap.com (placeholder)
- Preview: https://fakturasnap-preview.vercel.app (placeholder)

## Lokala kommandon
```bash
npm install
npm run dev
npm run test
```

## Kritiska kodområden
- `apps/web/src/app/(dashboard)` – kundflöde och Boris-knappen
- `packages/ocr-service` – OCR-adapters mot Sverige/Tyskland
- `packages/payments` – integration mot bank/IBAN

## Felsökning & drift
- Vercel env vars: `NEXT_PUBLIC_APP_URL`, `DATABASE_URL`, `OCR_API_KEY`
- Deploy logs: Vercel dashboard → Deploy details → "Functions"
- DB connect: Neon → FakturaSnap DB → read/write credentials
- Auth keys: Clerk/NextAuth (placeholder), lagras bara i Vercel secrets

## Noteringar
- Boris-komponenten måste kunna växla copy (enligt beslut FS-DEC-003)
- OCR-jobb bör köras via serverless queue (verifiera rate limits)
