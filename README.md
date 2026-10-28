# AI Agent Arena — NEXT AI Hackathon

**Status:** pregătire înainte de briefing. Acesta este un plan de lucru, **nu** cerința oficială a organizatorilor.

## Ideea de MVP (provizorie)

O aplicație care arată, transparent, cum trei roluri AI verifică o idee sau o soluție:

1. **Proposer** — propune un răspuns / o soluție.
2. **Challenger** — caută ipoteze slabe, contraexemple și teste.
3. **Judge** — compară argumentele și produce un verdict explicat.

În interfață utilizatorul vede inputul, pașii, criticile, verdictul și (când sunt disponibile) durata și costul. Scopul este **calitatea verificabilă**, nu doar o conversație spectaculoasă între boți.

**Regulă:** nu pretindem că rezultatele din modul demonstrativ sunt apeluri reale la AI. Etichetăm clar „Demo / simulated” până când există integrare reală.

## Priorități

- Un singur flux cap-coadă funcțional, înainte de funcționalități suplimentare.
- Vibe coding cu Lovable / Codex / ChatGPT, cu teste manuale după fiecare pas.
- API keys numai în secrete de server, niciodată în browser sau GitHub.
- Un set mic de cazuri de test pentru a compara răspunsul simplu cu răspunsul verificat adversarial.
- Ajustăm proiectul imediat ce primim challenge-ul oficial și criteriile de jurizare.

## Începe aici

- [Pașii pentru prima oră](docs/START_HERE.md)
- [Specificația MVP și criteriile de acceptare](docs/PRODUCT_SPEC.md)
- [Prompt pentru primul prototip în Lovable](docs/LOVABLE_PROMPT.md)
- [Prompt pentru Codex când avem codul aplicației](docs/CODEX_PROMPT.md)
- [Lucrul în echipă și planul de 48 de ore](docs/TEAM_PLAYBOOK.md)

## GitHub și Lovable

Acest repository a fost creat înaintea proiectului Lovable. Conform documentației Lovable, Git sync **creează un repository nou** și nu poate conecta direct unul existent. Prin urmare, aici ținem inițial planul și task-urile. Dacă Lovable creează alt repository pentru aplicație, alegem **un singur repository de cod principal** și mutăm documentația acolo, în loc să dezvoltăm două aplicații separate.

## Atenție la secrete

Repository-ul este **public**. Nu încărcați tokenuri, API keys, fișiere `.env`, date personale sau capturi care expun credențiale.

---
Actualizați această pagină după briefing.