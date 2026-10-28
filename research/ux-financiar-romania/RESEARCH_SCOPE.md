# Research: UX financiar accesibil pentru România

**Status:** ipoteze și întrebări de cercetare, NU cerințe finale și NU concluzii validate.

## Contextul proiectului

Challenge Stripe: cum facem navigarea viitorului financiar mai accesibilă, relevantă și utilă pentru oamenii din România.

Echipa explorează o aplicație cu două capabilități majore:

1. **Asistent conversațional financiar**, în română, cu răspunsuri substanțiale și explicate, întrebări de clarificare relevante, surse verificabile și ghidaj pentru obiective viitoare (ex. economisire pentru vacanță, buget lunar). Interacțiunea poate fi text și, doar dacă merită, voce.
2. **Analiza cheltuielilor**, inclusiv dintr-un extras bancar furnizat voluntar: categorii precum alimente, socializare și cheltuieli opționale, grafice ușor de înțeles, explicații, comparații și scenarii orientative.

**Rolul acestei zone de research:** ce vede și înțelege utilizatorul, ce îl face să aibă încredere, ce îl derutează și cum prezentăm rezultatele. Nu înlocuiește deciziile de produs ale colegilor.

## Ipoteze de testat, nu stereotipuri

- Unii utilizatori din România pot avea neîncredere în servicii financiare digitale; experiențele istorice, inclusiv cele din perioada comunistă, ar putea influența percepțiile unor segmente, dar amploarea și mecanismele trebuie verificate din cercetări.
- Unii utilizatori mai în vârstă sau cu competențe digitale reduse pot avea dificultăți cu meniuri, jargon și interfețe aglomerate; nu presupunem că toți vârstnicii au aceleași nevoi.
- O experiență orientată pe **citire și conversație**, cu puține acțiuni clare în context, poate funcționa mai bine decât onboarding pop-up-uri și dashboard-uri încărcate; trebuie testată, nu presupusă.

## Întrebări de cercetare prioritare

1. **Utilizatori și încredere:** ce dovezi există despre alfabetizarea financiară, încrederea în instituții/servicii digitale și competențele digitale în România, segmentate pe vârstă? Ce dovezi există, dacă există, despre efectele moștenirii comunismului asupra comportamentelor financiare actuale?
2. **UX și accesibilitate:** ce modele de interfață funcționează pentru persoane cu experiență digitală redusă? Cum aplicăm limbaj clar, progressive disclosure, control al ritmului, contrast, text lizibil, corectarea greșelilor și standarde WCAG?
3. **Conversational UX:** cum proiectăm un asistent inspirat de lizibilitatea Perplexity, dar nu o copie: răspuns direct, surse, exemple, întrebări de clarificare doar când contează, sugestii de continuare în context, evitarea întrebărilor repetitive „vrei să fac asta?”?
4. **Explicații și predicții:** cum diferențiem fapte, date introduse, presupuneri, calcule și proiecții? Cum evităm recomandări financiare personalizate nejustificate, certitudini false și afirmații fără sursă?
5. **Documente și confidențialitate:** ce poate fi extras local din PDF/CSV; cum recunoaștem și mascăm IBAN, nume, CNP, adrese, solduri/identificatori înainte de orice apel extern; ce riscuri rămân după redactare; ce necesită acord, stocare minimă, ștergere, transparență? Nu presupunem că simpla mascarea datelor face automat informația anonimă sau conformă GDPR.
6. **Analiza cheltuielilor:** categorii intuitive în context românesc; reguli de clasificare explicabile; tranzacții ambigue, transferuri între conturi, cash, refund-uri, comercianți neclari; cum evităm judecățile moralizatoare de tip „cheltuiești prea mult”?
7. **Voce:** merită în MVP? Cost, latență, confidențialitate, erori la sume în lei, accesibilitate și fallback text.
8. **Validare:** ce teste scurte de comprehensiune, task completion, încredere și usability putem face în timpul hackathonului?

## Scenarii reprezentative de validat

- „Vreau să strâng 4.000 lei pentru o vacanță în 8 luni. Cât să pun deoparte și ce se schimbă dacă într-o lună nu pot?”
- „Am încărcat un extras. Ce cheltuieli recurente am și ce concluzii sunt sigure versus presupuse?”
- „Nu înțeleg graficul. Explică-mi fără termeni financiari.”
- „Nu vreau să încarc un extras. Pot folosi aplicația doar cu sume introduse manual?”
- „De unde știi asta? Ce date ai folosit? Pot șterge documentul?”

## Rezultatele așteptate din research

- surse și statistici verificabile pentru România, cu limitele lor;
- 2–3 persona bazate pe dovezi, fără stereotipuri;
- principii de UX conversațional și de explicare a rezultatelor;
- recomandare argumentată pentru fluxul de încărcare și protecție a extraselor;
- exemple concrete de mesaje, întrebări și output-uri financiare;
- matrice impact/efort pentru un MVP de hackathon;
- protocol de testare cu utilizatori.

## Reguli pentru implementare ulterioară

- Nu colectăm date bancare reale în cercetare sau în demo fără necesitate și protecții adecvate; preferăm extrase sintetice.
- Nu trimitem documente brute sau chei API la un model extern implicit.
- Orice analiză financiară trebuie să arate limitele și ipotezele.
- Confirmăm regulile exacte despre AI pentru challenge-ul Stripe cu mentorii.
- Nu implementăm nimic doar fiindcă există credite Featherless/Lovable.
