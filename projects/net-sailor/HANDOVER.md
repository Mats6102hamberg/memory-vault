# Net Sailor – Handover

## Repo & deploy
- GitHub: https://github.com/mats-hamberg/net-sailor (placeholder)
- Production: https://netsailor.app (placeholder)
- Preview: https://netsailor-preview.vercel.app (placeholder)

## Lokala kommandon
```bash
npm install
npm run dev
npm run lint
```

## Kritiska kodområden
- `apps/web/src/app/(guardian)` – UI för trygghetsvarningar och Boris scenarion
- `apps/extension` – Browser extension som samlar telemetri
- `packages/risk-engine` – Poängsättning av risknivå för sidor

## Felsökning & drift
- Vercel env vars: `NEXT_PUBLIC_GUARDIAN_API`, `DATABASE_URL`
- Deploy logs: Vercel dashboard → Net Sailor projekt
- DB connect: Neon → Net Sailor DB
- Auth keys: använd Clerk/NextAuth (placeholder) lagrad i Vercel secrets

## Noteringar
- Boris måste synas i varje kritiskt steg (se NS-DEC-001)
- Riskmotor kräver regelbundna uppdateringar av blocklistor
