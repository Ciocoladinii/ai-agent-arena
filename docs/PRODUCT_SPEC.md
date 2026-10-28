# MVP — propunere, de confirmat după briefing

## Problema
Un singur model poate da un răspuns plauzibil dar greșit. Vrem să facem criticile și reviziile vizibile și comparabile.

## Flux utilizator
1. Utilizatorul introduce o idee, afirmație sau soluție.
2. Proposer răspunde cu o propunere și ipoteze explicite.
3. Challenger formulează 2–4 obiecții verificabile / contraexemple.
4. Proposer poate revizui o singură dată.
5. Judge oferă verdict, incertitudini și recomandări de verificare.
6. UI afișează separat fiecare etapă.

## Criterii de acceptare
- Un exemplu complet funcționează fără refresh.
- Stări loading, eroare și input gol.
- Verdictul nu este prezentat ca adevăr absolut.
- Modul simulat este marcat clar; modul AI real se activează numai după conectarea securizată a unui API.
- Cel puțin 3 scenarii de test cu comportament așteptat, inclusiv o afirmație intenționat falsă.
- Datele dintr-o sesiune nu sunt expuse altor utilizatori.

## Ce NU facem în MVP
- Execuție arbitrară de cod trimis de utilizator.
- Sisteme distribuite de agenți, cozi, containere multiple.
- Scoring științific inventat sau pretins ca măsură obiectivă.
- Login, plăți sau dashboard administrativ.

## Extensii doar dacă există timp
- Mod comparativ: single-agent vs arena.
- Afișare cost/timp real pe etapă.
- Test suite și rubrică de evaluare cu exemple verificabile.
- Export rezultat.

## Decizii deschise
- Stack și provider AI după validarea cu Lovable și regulamentul.
- Repository unic de cod după exportul Lovable.
- Limitele de cost și rate limiting.
