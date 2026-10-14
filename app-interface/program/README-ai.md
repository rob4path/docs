# Baza de cunoștințe „Program" — note pentru cine o publică

Conținutul acestui folder este documentație publică în limba română despre modulul de programare (Program) din TEAMM.
Este scris pentru două categorii de cititori: personalul centrelor și asistenții AI (ChatGPT, Claude, Gemini) pe care
personalul îi întreabă „cum fac X?".

## Publicare

Paginile din acest folder sunt incluse în navigația din `mint.json`. Când adaugi sau elimini o pagină, actualizează și `app-interface/program/_navigation.json`. Nu publica `onboarding/schedule.mdx`: descrie fluxul vechi.

## Convenții pentru pagini noi sau modificate

- Frontmatter cu `title` în română. Titlul spune direct ce explică pagina.
- Prima linie: `**Unde:** … (/admin/...)`.
- Etichetele din interfață se citează exact, cu ghilimele românești „…".
- Fără capturi de ecran: se învechesc, iar asistenții AI citesc textul.
- Sursele textelor: fișierele `*.entity-info.ts`, `scheduling-config.tooltips.ts` și `schedule-verify.catalog.ts` / `.text.ts` din codul aplicației. Când se schimbă un text acolo, actualizează pagina corespunzătoare.

## Test de regăsire

În Claude sau ChatGPT: lipește adresa unei pagini și pune trei întrebări pe care le-ar pune personalul.
Apoi adaugă conectorul MCP `https://help.teamm.work/mcp` și pune aceleași întrebări fără adresă. Răspunsurile trebuie să
folosească etichetele din interfață și să trimită la pagina corectă.
