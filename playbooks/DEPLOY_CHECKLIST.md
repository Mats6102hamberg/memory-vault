# Deploy-checklista

Denna checklista används inför varje deploy till Vercel.

## Före deploy
- [ ] Uppdatera `projects/<namn>/NOW.md`
- [ ] Säkerställ att alla beslut är dokumenterade
- [ ] Kör `npm run lint` och `npm run test`
- [ ] Verifiera att `.env.local` matchar Vercel Environment

## Vercel env vars
- [ ] `DATABASE_URL`
- [ ] `NEXT_PUBLIC_APP_URL`
- [ ] API-nycklar för tredjepart (OCR, auth, etc.)
- [ ] Kontrollera att Preview/Production har rätt värden

## Deploy
- [ ] Merge till `main`
- [ ] Trigger Vercel deploy (auto via Git)
- [ ] Övervaka build-loggar för varningar/fel

## Efter deploy – smoke tests
1. Öppna produktion → logga in → kör huvudflödet
2. Testa kritiska API-routes med curl eller Thunder Client
3. Kontrollera Boris-komponenten (om projektet använder den)
4. Uppdatera `logs/CHANGELOG.md` med datum + kort not
5. Bekräfta i Memory Vault att deploy är live
