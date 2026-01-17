# FakturaSnap – Decisions

## FS-DEC-001
- Datum: 2026-01-10
- Beslut: MVP lanseras i Sverige och Tyskland först
- Varför: Fokus på två marknader med liknande krav innan expansion
- Konsekvens: Övriga länder skjuts upp och kräver egna lokaliseringar

## FS-DEC-002
- Datum: 2026-01-12
- Beslut: Standardpipeline Next.js → GitHub → Vercel → Neon (Vercel DB) för hobby
- Varför: Minimera driftkomplexitet och få snabb deployloop
- Konsekvens: Alla miljöer måste följa denna struktur, inga specialfall

## FS-DEC-003
- Datum: 2026-01-15
- Beslut: Boris-knappen evolverar från "Boris – finns här för dig" → "Boris" → "B"-ikon
- Varför: Bygga igenkänning stegvis och kunna skala till små ytor
- Konsekvens: UI måste ha komponent som kan byta copy beroende på kontext
