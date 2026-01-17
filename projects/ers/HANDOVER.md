# ERS – Handover

## Repo & deploy
- GitHub: https://github.com/mats-hamberg/ers (placeholder)
- Production: https://ers-secure.com (placeholder)
- Preview: https://ers-preview.vercel.app (placeholder)

## Lokala kommandon
```bash
npm install
npm run dev
npm run check
```

## Kritiska kodområden
- `apps/control-center` – UI för admin + on-prem drift
- `services/ollama-runner` – wrapper runt Ollama inference
- `packages/security-policies` – policys och audits

## Felsökning & drift
- Vercel env vars: `NEXT_PUBLIC_PANEL_URL`, `DATABASE_URL`
- Deploy logs: Vercel dashboard → ERS projekt
- DB connect: Neon → ERS DB (om moln behövs för metadata)
- Auth keys: eget auth-system eller Clerk, lagrat i kundmiljö

## Noteringar
- On-prem drift kräver offline-licenser och dokumenterade playbooks
- All data måste kunna exporteras till kundens egna backup-system
