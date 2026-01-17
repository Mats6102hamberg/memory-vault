# Hur du använder Memory Vault

Memory Vault är din fasta rutin för varje ny chat-tråd, utvecklingssession och handover. Följ stegen nedan utan undantag.

## Workflow för ny chat-tråd
1. Öppna `start-here/START.md` och läs igenom relevanta projektsektioner
2. Kopiera in följande text i första meddelandet till agenten:
   - "Jag arbetar i projekt <namn>. Läs Memory Vault först. Utgå från projects/<namn>/NOW och DECISIONS."
3. Länka till berörda filer (NOW, DECISIONS, HANDOVER)
4. Ange var du vill börja och var du vill sluta

## Under pågående session
1. Beskriv alltid vad som ändras och varför
2. Uppdatera filer kontinuerligt – hellre små commit-steps än stora
3. Vid nya beslut, skriv direkt in dem i `DECISIONS.md`
4. Vid större framsteg, lägg post i `logs/CHANGELOG.md`

## Efter varje session (obligatoriskt)
1. Uppdatera projektets `NOW.md`
   - Status, fokus, nästa 3 actions, blockers
2. Om beslut fattades: uppdatera `DECISIONS.md`
3. Revidera `HANDOVER.md` om onboardinginfo ändrats
4. Lägg till datum + notering i `logs/CHANGELOG.md`
5. Commit + push

## Golden rule
- Hellre 5 rader tydligt än 500 rader oklart
- Inga placeholders utan förklaring
- Uppdatera `NOW` först, därefter `DECISIONS` om det finns nya beslut

## Översikt av filer att uppdatera
- `projects/<namn>/NOW.md`
- `projects/<namn>/DECISIONS.md`
- `projects/<namn>/HANDOVER.md`
- `projects/<namn>/LINKS.md`
- `logs/CHANGELOG.md`

Följ denna rutin varje gång för att hålla minnesbanken pålitlig.
