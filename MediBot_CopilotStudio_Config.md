# MediBot — Copilot Studio Config

Everything I set up for the chatbot. This is the reference doc I used while building it in Copilot Studio.

---

## Description

MediBot is EduConnect's chatbot. It helps parents and students find tutors, check pricing, and book sessions. All conversations are in Romanian. Built with Microsoft Copilot Studio.

---

## Instructions

This goes into Settings → Instructions in Copilot Studio:

```
Ești MediBot, asistentul virtual al EduConnect — o platformă de meditații particulare din România.

REGULI GENERALE:
- Răspunzi DOAR în limba română, indiferent de limba în care ți se scrie.
- Tonul tău este prietenos, profesionist și empatic. Te adresezi cu "dumneavoastră" părinților și cu "tu" elevilor.
- Dacă nu știi un răspuns, spui sincer și oferi alternative (contact telefonic, email, sau callback).
- Nu inventezi informații despre profesori, disponibilitate sau prețuri care nu sunt în baza ta de cunoștințe.
- Când un utilizator vrea să rezerve o ședință, colectezi: numele elevului, clasa, materia, preferința de program (dimineață/după-amiază/seară), și dacă preferă online sau fizic.

PERSONALITATE:
- Folosești emoji-uri moderat (✅, 📚, 📅, ⏰) pentru claritate, nu exces.
- Ești concis — răspunsuri de 2-4 propoziții unde e posibil.
- La finalul fiecărui răspuns, oferi un follow-up natural (ex: "Doriți să vedeți și prețurile?" sau "Vreți să rezervăm o ședință de probă?").

LIMITĂRI:
- Nu oferi sfaturi medicale, psihologice sau legale.
- Nu discuți despre competitori.
- Nu procesezi plăți direct — redirecționezi spre pagina de plată sau contactul EduConnect.
- Nu partajezi date personale ale profesorilor (telefon, email personal).
```

---

## Knowledge Base

Uploaded as separate .txt files in Copilot Studio → Knowledge → Files.

### general.txt

```
DESPRE EDUCONNECT

EduConnect este o platformă de meditații particulare din București, România.
Oferim meditații pentru elevi care se pregătesc pentru Evaluarea Națională (clasa a 8-a) și Bacalaureat (clasa a 12-a).

Forma de lucru: online (Google Meet / Zoom) sau fizic (la domiciliul elevului sau la sediul EduConnect).
Program: Luni - Sâmbătă, 09:00 - 21:00.
Ședința standard: 60 minute (se pot rezerva și blocuri de 90 sau 120 de minute).
Ședință de probă: GRATUITĂ (prima ședință cu orice profesor nou, 30 de minute).

Contact:
Telefon: 0712 345 678
Email: contact@educonnect.ro
Website: www.educonnect.ro
Adresa sediu: Str. Exemplu nr. 10, Sector 1, București

Politică de anulare:
Anulare gratuită cu minim 24 de ore înainte.
Anulare cu mai puțin de 24 de ore: se percepe 50% din tarif.
Neprezentare fără anulare: se percepe tariful integral.
```

### subjects-tutors.txt

```
MATERII DISPONIBILE

EVALUAREA NAȚIONALĂ (clasa a 5-a - a 8-a):
Matematică
Limba și Literatura Română

BACALAUREAT (clasa a 9-a - a 12-a):
Matematică (M1 - mate-info / M2 - științe / M3 - pedagogic)
Limba și Literatura Română
Fizică
Chimie
Biologie
Informatică (C/C++, Python)
Istorie
Geografie
Logică
Economie
Limba Engleză
Limba Franceză

PROFESORI EDUCONNECT

1. Prof. Andrei Popescu — Matematică (EN + BAC M1/M2)
Experiență: 12 ani, Rating: 4.9/5, Disponibilitate: L-V 14:00-20:00
Stil: structurat, exerciții progresive, simulări de examen
Disponibil: online + fizic

2. Prof. Maria Ionescu — Limba și Literatura Română (EN + BAC)
Experiență: 8 ani, Rating: 4.8/5, Disponibilitate: L-S 10:00-18:00
Stil: interactiv, accent pe eseuri și analiză de text
Disponibil: online + fizic

3. Prof. Vlad Dumitrescu — Fizică (BAC)
Experiență: 10 ani, Rating: 4.7/5, Disponibilitate: L-V 16:00-21:00
Stil: explicații vizuale, probleme aplicate, experimente mentale
Disponibil: doar online

4. Prof. Elena Radu — Chimie (BAC)
Experiență: 6 ani, Rating: 4.8/5, Disponibilitate: L-S 09:00-15:00
Stil: scheme rezumat, exerciții tip grilă, recapitulări rapide
Disponibil: online + fizic

5. Prof. Bogdan Stanciu — Informatică C++ / Python (BAC)
Experiență: 5 ani, Rating: 4.9/5, Disponibilitate: L-V 17:00-21:00, S 10:00-14:00
Stil: learning by doing, mini-proiecte, debugging live
Disponibil: doar online

6. Prof. Ana Marin — Limba Engleză (BAC + conversație)
Experiență: 9 ani, Rating: 4.6/5, Disponibilitate: L-V 10:00-19:00
Stil: imersiv, accent pe speaking și writing
Disponibil: online + fizic

7. Prof. Cristian Neagu — Istorie (BAC)
Experiență: 7 ani, Rating: 4.7/5, Disponibilitate: M-S 12:00-20:00
Stil: narativ, cronologii vizuale, eseuri structurate
Disponibil: online + fizic

8. Prof. Ioana Pavel — Biologie (BAC)
Experiență: 4 ani, Rating: 4.5/5, Disponibilitate: L-V 14:00-19:00
Stil: scheme, diagrame, quiz-uri rapide
Disponibil: doar online
```

### pricing.txt

```
MODEL DE PREȚURI EDUCONNECT

EVALUAREA NAȚIONALĂ (clasele 5-8):
Matematică — 100 RON / oră
Limba și Literatura Română — 90 RON / oră

BACALAUREAT (clasele 9-12):
Matematică (M1) — 130 RON / oră
Matematică (M2/M3) — 120 RON / oră
Limba și Literatura Română — 100 RON / oră
Fizică — 120 RON / oră
Chimie — 110 RON / oră
Biologie — 100 RON / oră
Informatică (C++/Python) — 130 RON / oră
Istorie — 90 RON / oră
Geografie — 90 RON / oră
Logică / Economie — 90 RON / oră
Limba Engleză — 100 RON / oră
Limba Franceză — 100 RON / oră

PACHETE ȘI REDUCERI:
Pachet 10 ședințe: 10% reducere din prețul total.
Pachet 20 ședințe: 15% reducere din prețul total.
Pachet frați/surori: 10% reducere pentru al doilea copil, cumulabil cu pachetele.
Ședință de probă: gratuită, 30 de minute, o singură dată per profesor.

SESIUNI INTENSIVE (perioadele pre-examen):
Disponibile în lunile aprilie-iunie.
Pachete de 3 ședințe pe săptămână cu un discount suplimentar de 5%.
Se rezervă cu minim 2 săptămâni în avans.

MODALITĂȚI DE PLATĂ:
Transfer bancar, card (prin link de plată securizat) sau cash (doar pentru ședințele fizice).
Factura se emite automat după fiecare plată.
```

### faq.txt

```
ÎNTREBĂRI FRECVENTE

Î: Cum funcționează ședința de probă?
R: Prima ședință cu orice profesor nou este gratuită și durează 30 de minute. Scopul este să vedeți dacă stilul profesorului se potrivește cu nevoile elevului. Nu există nicio obligație de continuare.

Î: Pot schimba profesorul?
R: Da, oricând. Puteți solicita un alt profesor pentru aceeași materie fără costuri suplimentare. Prima ședință cu noul profesor este tot gratuită.

Î: Cum se desfășoară ședințele online?
R: Prin Google Meet sau Zoom. Profesorul trimite linkul cu 15 minute înainte de oră. E nevoie doar de un laptop/tabletă cu cameră și microfon.

Î: Ce se întâmplă dacă elevul nu înțelege o lecție?
R: Profesorul poate relua oricând un subiect. Nu se avansează până când elevul nu se simte confortabil. Sesiunile sunt personalizate pe ritmul fiecărui elev.

Î: Oferiți materiale de studiu?
R: Da. Fiecare profesor oferă fișe de lucru, rezumate și teste de antrenament incluse în prețul ședinței.

Î: De câte ședințe pe săptămână am nevoie?
R: Depinde de nivel și obiective. Recomandăm: menținere — 1 ședință/săptămână, pregătire examen (cu 6+ luni) — 1-2 ședințe/săptămână, intensiv pre-examen (ultimele 2-3 luni) — 2-3 ședințe/săptămână.

Î: Pot plăti în rate?
R: Pachetele de 10 și 20 de ședințe se plătesc integral la achiziție. Pentru planuri personalizate de plată, contactați-ne la contact@educonnect.ro.

Î: Aveți profesori și pentru clasele primare?
R: Momentan, EduConnect acoperă clasele 5-12, cu focus pe Evaluarea Națională și BAC. Urmează să extindem oferta și pentru clasele 1-4.

Î: Unde se țin ședințele fizice?
R: La sediul EduConnect (Str. Exemplu nr. 10, Sector 1, București) sau la domiciliul elevului (doar în București, fără cost suplimentar de deplasare).
```

---

## Trigger Phrases

These go into each topic's trigger list in Copilot Studio.

**Informații generale:** ce este educonnect, cine sunteți, ce oferiți, vreau informații, despre voi, cum funcționează, ce faceți, meditații particulare

**Prețuri:** cât costă, ce prețuri aveți, tarife, preț meditații, cât e ora, pachet reducere, oferte, discount

**Materii:** ce materii aveți, la ce materii, predați matematică, aveți fizică, ce se poate învăța, materii disponibile, pregătire bac, pregătire evaluare națională

**Profesori:** cine predă, ce profesori aveți, vreau un profesor de, recomandați un profesor, cel mai bun profesor, schimb profesorul, alt profesor, profesori disponibili

**Rezervare:** vreau să rezerv, programare, rezervare, vreau o ședință, booking, când pot veni, program disponibil, ședință de probă, prima ședință

**Anulare / Reprogramare:** vreau să anulez, anulare, reprogramare, mut ședința, schimb data, nu mai pot veni, amân ședința

**Online vs fizic:** online sau fizic, cum se face online, unde se țin ședințele, aveți și online, locația, adresa, sediu

**FAQ:** întrebări frecvente, materiale de studiu, câte ședințe, schimb profesor, plata în rate, cum plătesc, factură

---

## Conversation Flows

How the bot should handle each main scenario.

**Greeting**
Bot says hi, mentions its name, lists what it can help with (subjects, pricing, booking), asks what the user needs.

**Pricing**
Asks if the user is preparing for EN or BAC → shows prices for the relevant level → mentions packages and discounts → offers to show available tutors or book a session.

**Tutor Matching**
Asks what subject → asks EN or BAC → shows matching tutors with rating, style, availability → offers to book a free trial.

**Booking**
Collects step by step: student name → class → subject → shows available tutors, user picks one → online or fizic → preferred time slot → confirms the reservation with a summary.

**Cancellation / Reschedule**
Asks if they want to cancel or reschedule → if cancel, reminds about the 24h policy → if reschedule, shows alternative slots → confirms.

**Free Trial**
Explains it's free, 30 min, one per tutor, no obligation → collects subject, level, online/fizic preference → recommends a tutor → books the trial.

**Escalate**
Tells the user it can't transfer to a human right now → gives phone and email → mentions response time.

---

## Suggested Prompts

These show up as buttons when someone opens the chat:

📚 Ce materii aveți disponibile?
💰 Cât costă o ședință de meditații?
📅 Vreau să rezerv o ședință
🎯 Ajută-mă să găsesc un profesor potrivit

---

## Pricing Rationale

Prices are based on the Bucharest private tutoring market (2025-2026). Math M1 and Informatică are at the top (130 RON) because demand is high and tutor supply is lower. Humanities sit at 90 RON, which matches what most tutors charge. The free 30 min trial is there to lower the barrier — parents want to see the tutor before committing. Packages (10 and 20 sessions) give discounts to encourage longer commitments.
