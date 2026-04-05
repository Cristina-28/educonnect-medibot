MediBot — Testing
Testing done in the Copilot Studio Test Chat panel. All interactions are in Romanian.
Date: 05.04.2026
---
System Topics


01 — Greeting
Input: `salut`
Expected: Romanian greeting with bot name
Actual: Salut! 👋 Mă bucur să te văd aici. Te pot ajuta să găsești un profesor, să afli prețurile sau să rezervi o ședință. Ce ai dori să faci? 📚
Status: Good, needs improvement (mention bot name)
![screenshot](screenshots/test-01-greeting.png)


02 — Thank You
Input: `mulțumesc`
Expected: "Cu plăcere" response
Actual: Cu plăcere! 😊 Dacă mai ai nevoie de ceva, sunt aici.
Status: Good
![screenshot](screenshots/test-02-thankyou.png)


03 — Escalate
Input: `vreau să vorbesc cu cineva`
Expected: Message with phone and email
Actual: Momentan nu am posibilitatea să te transfer la un operator, dar poți contacta echipa EduConnect direct la 📞 0712 345 678 sau 📧 ​contact@educonnect.ro​.
Status: Good
![screenshot](screenshots/test-03-escalate.png)


04 — Reset
Input: `o luăm de la început`
Expected: Asks for confirmation before resetting
Actual: Ești sigur că vrei să reîncepi conversația?
Status: Good
![screenshot](screenshots/test-04-reset.png)


05 — Fallback
Input: `asjkdhaskd`
Expected: Asks to rephrase
Actual: Nu sunt sigur că am înțeles mesajul tău. 😊 Te pot ajuta cu informații despre meditații, profesori sau programări. Despre ce ai vrea să discutăm?
Status: Good
![screenshot](screenshots/test-05-fallback.png)
---



Knowledge Base

06 — Subjects
Input: `ce materii aveți?`
Expected: List of EN + BAC subjects
Actual: Avem o gamă variată de materii pentru toate nivelurile școlare ✅. Cele mai solicitate sunt:

Matematică
Română
Engleză
Franceză
Informatică
Fizică și Chimie
Biologie
Putem acoperi și alte discipline la cerere. 📚
Vrei să îți trimit lista completă sau să verificăm disponibilitatea pentru o materie anume?
Status: Good
![screenshot](screenshots/test-06-subjects.png)


07 — Pricing
Input: `cât costă matematica pentru BAC?`
Expected: 130 RON (M1) / 120 RON (M2)
Actual: Pentru pregătirea la matematică pentru Bacalaureat pe platforma EduConnect, tarifele sunt următoarele:

Matematică M1 (mate-info): 130 RON / oră
Matematică M2/M3 (științe sau pedagogic): 120 RON / oră
✅ Reduceri disponibile:

Pachet 10 ședințe: -10%
Pachet 20 ședințe: -15%
Frați/surori: -10% pentru al doilea copil (cumulabil cu pachetele)
Ședință de probă gratuită (30 min, o singură dată per profesor)
💡 În perioada aprilie-iunie avem și sesiuni intensive (3 ședințe/săptămână) cu discount suplimentar de 5%​1​.

Doriți să vă trimit și programul profesorilor disponibili sau facem direct o rezervare pentru o ședință de probă? 📅
Status: Good
![screenshot](screenshots/test-07-pricing.png)


08 — Tutor Match
Input: `ce profesori predau fizică?`
Expected: Vlad Dumitrescu + details
Actual: Am găsit informațiile pentru tine! ✅

Profesorii care predau fizică pe EduConnect:

Prof. Vlad Dumitrescu — specializat în Fizică pentru Bacalaureat
Experiență: 10 ani
Rating: 4.7/5
Disponibilitate: Luni - Vineri, 16:00 - 21:00
Stil: explicații vizuale, probleme aplicate, experimente mentale
Format: doar online​1​
Doriți să vă spun și tariful pentru fizică sau să rezervăm o ședință de probă gratuită? 📅
Status: Good
![screenshot](screenshots/test-08-tutor.png)


09 — Free Trial
Input: `aveți ședință de probă?`
Expected: Free, 30 min, one per tutor
Actual: Da, oferim ședințe de probă pentru majoritatea materiilor ✅. Acestea sunt o ocazie excelentă să cunoști profesorul și stilul de predare înainte de a continua.

Vrei să îți rezerv acum o ședință de probă? 📅 Dacă da, am nevoie de:

Numele elevului
Clasa
Materia dorită
Preferința de program (dimineață/după-amiază/seară)
Online sau fizic
Cum dorești să procedăm?
Status: Good, might need improvement (doesn't mention 30 min + one per tutor)
![screenshot](screenshots/test-09-trial.png)


10 — Payment
Input: `cum plătesc?`
Expected: Transfer, card, cash (fizic only)
Actual: Plata se face foarte simplu ✅:

Online, prin card bancar, direct pe platforma EduConnect, după ce confirmați rezervarea.
Transfer bancar, dacă preferați această opțiune (detaliile apar în contul dumneavoastră după rezervare).
Doriți să vă trimit linkul către pagina de plată sau să facem mai întâi o rezervare pentru ședință? 📅
Status: Good, needs improvement(doesn't mention cash)
![screenshot](screenshots/test-10-payment.png)
---


Edge Cases

11 — English Input
Input: `hello`
Expected: Still responds in Romanian
Actual: Bună! 👋 Sunt Medibot, asistentul virtual EduConnect. Te pot ajuta cu informații despre meditații, profesori, prețuri sau programări. Despre ce ai vrea să discutăm? 📚
Status: Good
![screenshot](screenshots/test-11-english.png)

12 — Cancellation
Input: `vreau să anulez`
Expected: Cancellation info request
Actual: Îmi pare rău să aud asta! ✅ Pot să te ajut să anulezi ședința programată. Te rog să îmi spui numele elevului și data/ora ședinței pentru a continua.

Vrei să reprogramezi ședința sau doar să o anulezi definitiv? 📅
Status: Good
![screenshot](screenshots/test-12-cancel.png)

13 — Booking
Input: `vreau să rezerv o ședință`
Expected: Step-by-step: name, class, subject, tutor, format, time
Actual: Super! 📚 Hai să facem rezervarea. Am nevoie de câteva detalii:

✅ Numele elevului
✅ Clasa
✅ Materia
✅ Preferința de program (dimineață / după-amiază / seară)
✅ Formatul (online sau fizic)

Îmi poți da aceste informații?
Status: Needs improvement
![screenshot](screenshots/test-13-booking.png)
---

Bugs
None yet. Will update as I test.
