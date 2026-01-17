# AI-agent workflow

Standardprocedur för alla agenter som arbetar i Mats ekosystem.

## Scope
1. Läs `projects/<namn>/NOW.md` och `DECISIONS.md`
2. Bekräfta uppdragets omfattning och förväntat resultat
3. Identifiera vilka filer som kommer ändras

## Utförande
- Jobba i tydliga steg
- Dokumentera antaganden i commit-meddelanden
- Använd Tailwind + App Router för UI (default)
- Skriv tester/loggar där det är rimligt

## Teststeg
1. `npm run lint`
2. `npm run test` (om finns)
3. Manuell kontroll av huvudflöden (lista minst 5 steg i DOSPROGRAM_CHECKLIST md om relevant)
4. Uppdatera `logs/CHANGELOG.md` efter verifiering

## Commit & dokumentation
- Commit-meddelande: `feat: <kort beskrivning>` eller `fix: ...`
- Push direkt efter commit
- Uppdatera Memory Vault: NOW → DECISIONS → HANDOVER
- Lägg till datum + sammanfattning i `logs/CHANGELOG.md`

## Efterarbete
- Skicka rapport med filer, tester, nästa steg
- Lämna tydliga förbättringsförslag
- Vänta på Mats feedback innan nya ändringar
