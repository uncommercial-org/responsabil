---
title: "Ce este un test de penetrare: tipuri, etape și cele mai cunoscute cazuri"
date: 2026-06-15
draft: false
description: "Aflați ce este un test de penetrare (pentest), cum se diferențiază de scanarea vulnerabilităților și care sunt cele mai răsunătoare cazuri reale de hacking etic."
categories: ["securitate"]
tags: ["securitate cibernetică", "pentest", "hacking etic", "vulnerabilități", "red team", "audit it"]
cover:
  image: "images/cybercalm/ce-este-un-test-de-penetrare-tipuri-etape-cazuri.webp"
  alt: "Ilustrație concept securitate cibernetică și hacking etic prin teste de penetrare"
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Zilnic, organizații din întreaga lume angajează hackeri pentru a le sparge propriile sisteme — să pătrundă în rețea, să ocolească protecția și să ajungă la cele mai valoroase date. Nu este un paradox: așa funcționează un test de penetrare (penetration testing, sau prescurtat pentest) — o imitare controlată a unui atac cibernetic real, comandată pentru a găsi vulnerabilități înainte ca atacatorii reali să o facă. Iar rezultatele pot fi neașteptate: de la spargerea unor sisteme aparent inexpugnabile în doar câteva ore, până la cazuri în care specialiștii înșiși au ajuns în spatele gratiilor.

## **Ce este un test de penetrare**

**Un test de penetrare** este un atac autorizat asupra propriului sistem, pe care specialiștii îl efectuează la cererea proprietarului acestuia, pentru a găsi vulnerabilități înainte ca infractorii reali să le exploateze. Clientul angajează o echipă de „hackeri etici”, stabilește ce anume au voie să atace, iar aceștia încearcă să depășească protecția folosind aceleași metode ca atacatorii reali: caută puncte slabe, le exploatează și documentează cât de departe au reușit să avanseze.

Obiectul testului poate fi orice: un site web, o rețea corporativă, o aplicație mobilă, puncte de acces wireless, angajații companiei (caz în care vorbim despre inginerie socială) sau chiar locații fizice — uși, încuietori, alarme și sisteme de control al accesului. Scopul este întotdeauna același: a vedea protecția prin ochii unui atacator și a obține o listă de breșe concrete care trebuie închise.

## **Cu ce se diferențiază de scanarea vulnerabilităților**

Testul de penetrare este adesea confundat cu scanarea vulnerabilităților, deși acestea sunt lucruri diferite. Scanarea este, în mare parte, un proces automatizat: un program special verifică sistemul pe baza unei baze de date cu probleme cunoscute și oferă o listă de potențiale puncte slabe. Acesta răspunde la întrebarea „ce ar putea fi teoretic periculos”.

Pentestul merge mai departe: specialistul încearcă manual să utilizeze real acele vulnerabilități pentru a demonstra riscul real de afaceri. Acesta răspunde la întrebarea „ce anume poate fi spart cu adevărat și la ce va duce acest lucru”. Ingeniozitatea umană, și nu doar automatizarea, este cea care distinge un test de calitate: echipele de top efectuează până la 95% din verificări manual, modelând acțiunile unui adversar real.

## **Cum s-a născut această profesie: de la „tiger teams” la red team**

Ideea de a ataca intenționat propriile sisteme a apărut încă de la începuturile erei computerelor. La sfârșitul anilor 1960 și începutul anilor 1970, corporația RAND, împreună cu agenția ARPA, a studiat securitatea primelor sisteme de acces partajat. Rezultatul a fost [raportul RAND R-609 „Security Controls for Computer Systems”](https://www.rand.org/pubs/reports/R609-1.html) (1970), cunoscut sub numele de „raportul Ware” după numele președintelui grupului de lucru, Willis Ware: acesta a descris pentru prima dată sistemic amenințarea de pătrundere în astfel de sisteme — de la hacking-ul „activ” la interceptarea „pasivă” — și a pus bazele industriei.

Tot atunci, guvernul și centrele de cercetare au început să formeze așa-numitele „echipe de tigri” (**tiger teams**) — grupuri de specialiști însărcinați să spargă protecția pentru a identifica și remedia breșele. În 1972, pionierul securității computerizate James P. Anderson a prezentat o metodologie pas cu pas a acestor verificări: găsirea vulnerabilității, construirea unui atac în jurul ei, verificarea acestuia și utilizarea lui pentru acces. Această logică stă la baza pentestului și în prezent. Un exemplu timpuriu notabil a fost testul sistemului MULTICS, efectuat de Forțele Aeriene ale SUA în 1974, care a scos la iveală breșe grave de securitate.

Ulterior, practica a depășit limitele structurilor militare și guvernamentale, iar în jurul ei s-au dezvoltat standarde și metodologii. Astăzi, specialiștii se bazează pe cadre recunoscute la nivel global — printre care PTES, OWASP Testing Guide, NIST SP 800-115, OSSTMM și matricea MITRE ATT&CK. În paralel, a apărut conceptul mai larg de **red team** (echipa roșie) — care nu mai înseamnă doar căutarea breșelor tehnice, ci o imitare completă a adversarului, combinând hacking-ul rețelelor, ingineria socială și pătrunderea fizică.

## **„Black box”, „white box” și „grey box”**

În funcție de cât de multă informație primește specialistul la început, testele sunt împărțite în trei tipuri:

*   **„Black box” (cutia neagră)** — testerul nu știe aproape nimic despre sistem, la fel ca un atacator extern real. Este cel mai realist scenariu, dar și cel mai lung: se consumă mult timp pentru recunoaștere.
*   **„White box” (cutia albă)** — specialistului i se oferă acces complet: scheme de rețea, documentație, chiar și codul sursă. Astfel, protecția poate fi verificată cât mai profund, fără a pierde timp cu recunoașterea.
*   **„Grey box” (cutia gri)** — o variantă de compromis: testerul are cunoștințe parțiale sau acces limitat. Acesta combină realismul „black box” cu profunzimea „white box”, fiind cel mai des ales în practică.

## **Cum se desfășoară un test tipic**

În ciuda diferențelor, majoritatea pentestelor parcurg etape similare:

**Pregătirea și stabilirea limitelor.** Clientul și executanții stabilesc clar ce anume poate fi atacat (scope), conform căror reguli și unde este linia roșie. Această etapă este cea mai importantă și, de cele mai multe ori, aici apar problemele despre care vom discuta.

**Recunoașterea.** Colectarea informațiilor despre țintă: domenii deschise, servicii, puncte de intrare, date despre angajați.

**Scanarea și analiza.** Căutarea vulnerabilităților specifice în sistemele identificate.

**Exploatarea.** Încercarea de a utiliza real breșele găsite și de a obține acces.

**Menținerea accesului.** Verificarea profunzimii la care se poate avansa în interiorul sistemului și dacă se poate menține accesul fără a fi detectat.

**Raportarea.** Rezultatul cheie al întregii munci: o listă de vulnerabilități, evaluarea criticității acestora și recomandări pentru remediere.

## **Când testul de penetrare nu merge conform planului**

Un pentest bun găsește aproape întotdeauna breșe — conform estimărilor specialiștilor, echipele roșii obțin acces profund la rețele în marea majoritate a cazurilor. Dar, uneori, cele mai interesante lucruri încep atunci când ceva nu merge conform planului. Iată câteva povești care au devenit clasice.

### Arestarea la tribunalul din statul Iowa

Ramura judiciară a statului a angajat compania Coalfire pentru a verifica securitatea fizică a tribunalelor. Doi dintre specialiștii săi, Gary DeMercurio și Justin Wynn, „spăsese” deja cu succes două clădiri când, în noaptea de 11 septembrie 2019, au ajuns la tribunalul din comitatul Dallas. Au găsit o ușă care era închisă, dar nu complet încuiată, au încuiat-o intenționat pentru a testa corect încuietoarea, apoi au deschis-o cu o unealtă improvizată — și au declanșat alarma. Apoi au făcut ceea ce fac întotdeauna în astfel de cazuri: au așteptat liniștiți poliția, având la ei scrisoarea de autorizare din partea clientului.

Această „scrisoare de exonerare de răspundere” nu a funcționat. Șeriful local i-a reținut pe amândoi, au fost acuzați de furt prin efracție și au petrecut aproape o zi în spatele gratiilor. Rădăcina problemei a fost organizatorică: administrația tribunalelor statului nu a avertizat poliția locală despre test, iar clădirea aparținea comitatului, astfel încât a apărut o dispută dacă autoritățile statului aveau dreptul să autorizeze pătrunderea într-o proprietate străină. Ulterior, acuzațiile au fost reduse la pătrundere ilegală, iar după audierile din legislativul statului — au fost retrase complet. Președintele Curții Supreme din Iowa chiar și-a cerut scuze deputaților, recunoscând că incidentul a subminat încrederea în sistemul judiciar.

Povestea a continuat ani de zile. DeMercurio și Wynn au dat în judecată comitatul pentru arestare ilegală și defăimare, iar abia în ianuarie 2026 — aproape șapte ani mai târziu — cazul s-a încheiat cu o [înțelegere amiabilă de 600.000 de dolari](https://www.kcrg.com/2026/01/30/cybersecurity-testers-reach-600000-settlement-after-wrongful-arrest/) — cu câteva zile înainte de începerea procesului și fără recunoașterea vinovăției de către comitat. Ambii testeri au fondat între timp propria companie, Kaiju Security. Iar prezentarea lor la conferința Black Hat a devenit o lecție amară pentru industrie: toate limitele testului trebuie fixate în scris și coordonate cu toți cei care ar putea chema poliția.

### Chiar și „cetățile” cad

În 2016, a devenit publică povestea modului în care una dintre cele mai „secrete” companii tehnologice din lume, Palantir, a fost practic învinsă de propria echipă de hackeri „albi”. Pentru publicul larg, a sunat ca o senzație, dar pentru industrie — ca o rutină. Echipele roșii înving aproape întotdeauna apărătorii și găsesc practic întotdeauna cel puțin câteva puncte slabe serioase. Paradoxul este că însuși faptul de a comanda un astfel de test este un semn al unei abordări mature a securității, nu al slăbiciunii.

### Camionul cu discuri și coborârea de pe acoperiș

Testele fizice generează multe situații aproape anecdotice. Specialistul experimentat Charles Henderson a povestit odată cum, ieșind dintr-un obiectiv după misiune, a văzut un camion plin cu discuri ale companiei, pregătite pentru distrugere — cu cheile în contact. L-a sunat pe manager și a întrebat dacă acest lucru intră „în limitele” testului. S-a dovedit că da. Într-un alt caz, o echipă australiană a fost reținută de poliție după ce au coborât în haine negre de pe acoperișul unui centru de date pe frânghii, cu camere pe cap. Aceste povești ilustrează bine regula principală: tot ceea ce specialistul intenționează să facă trebuie să fie autorizat în prealabil de client.

### O surpriză în managerul de parole

Uneori, testul aduce o surpriză chiar și specialiștilor. În timpul unui pentest, echipa RedTeam Pentesting a descoperit că implementarea autentificării prin Windows Hello în popularul manager de parole Bitwarden permitea furtul de la distanță al tuturor datelor salvate în seif — fără a cunoaște parola principală și fără autentificare biometrică. Descoperirea a fost atât de neașteptată încât, cu acordul clientului, specialiștii au [publicat o relatare separată](https://blog.redteam-pentesting.de/2024/bitwarden-heist/) despre aceasta. Bitwarden a remediat problema încă din aprilie 2023 (versiunea 2023.4.0), dar cazul ne amintește: chiar și produsele create pentru securitate au nevoie de verificări independente.

## **Ce ar trebui să rețină organizațiile**

Testul de penetrare este una dintre cele mai eficiente modalități de a verifica protecția în practică, nu pe hârtie. Dar povestea din Iowa arată că pregătirea tehnică este doar jumătate din treabă. Înainte de a comanda un pentest, merită să rețineți câteva principii:

*   Stabiliți clar limitele testului (scope) și fixați-le în scris — acordurile verbale nu protejează nici clientul, nici executantul.
*   Asigurați-vă că cel care dă autorizația are într-adevăr puterea de a face acest lucru, mai ales când este vorba de clădiri sau sisteme terțe.
*   Avertizați toți factorii implicați — de la serviciul de securitate până la poliția locală, dacă testul implică pătrundere fizică.
*   Nu uitați că scopul testului nu este de a „prinde” echipa într-un eșec, ci de a obține o imagine onestă a propriilor puncte slabe și de a avea timp să le corectați.

În cele din urmă, principalul paradox al pentestului este că succesul său se măsoară prin numărul de probleme găsite. Cu cât echipa angajată descoperă mai multe breșe, cu atât mai puține vor rămâne pentru atacatorii reali.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/test-na-proniknennia/?utm_source=responsabil) și a fost tradus în limba română.
