---
title: "6 servicii DNS securizate și gratuite: cum să îți criptezi traficul de internet"
date: 2026-03-23
draft: false
description: "Află cum să îți protejezi confidențialitatea online folosind servicii DNS securizate. Ghid pas cu pas pentru configurarea Google, Cloudflare, Quad9 și altele."
categories: ["securitate"]
cover:
  image: "images/cybercalm/6-servicii-dns-securizate-gratuite-criptare-trafic.jpg"
  alt: ""
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Majoritatea utilizatorilor sunt convinși că o protecție fiabilă a dispozitivului este asigurată de un antivirus, instrumente de detectare malware și un firewall. Aceste instrumente sunt într-adevăr importante — dar mai există un nivel de protecție despre care se uită adesea: DNS.

**DNS (Domain Name System, sistemul de nume de domeniu)** — este un fel de agendă telefonică a internetului. Când introduceți în browser o adresă precum google.com, DNS-ul este cel care transformă acest nume într-o adresă numerică pe care computerele o înțeleg — de exemplu, 142.250.203.206. Fără DNS, ar trebui să memorăm astfel de cifre în locul site-urilor obișnuite.

Traficul DNS obișnuit este transmis în formă deschisă: oricine interceptează conexiunea la internet poate vedea ce site-uri vizitează utilizatorul. Acest lucru este valabil chiar și pentru rețeaua Wi-Fi de acasă — furnizorul tău de internet vede, de asemenea, ce site-uri te interesează. Un DNS securizat criptează aceste interogări, făcându-le ilizibile pentru persoanele neautorizate.

## Cum să schimbi DNS-ul: instrucțiuni pas cu pas

Schimbarea serverului DNS nu este mai dificilă decât conectarea la Wi-Fi. Mai jos sunt instrucțiuni pentru cele mai populare platforme. Pentru exemplu, sunt folosite adresele Cloudflare DNS (1.1.1.1 și 1.0.0.1), dar aceiași pași sunt valabili pentru orice serviciu din lista de mai jos.

**Adresa IP sau numele gazdei: care este diferența**
La configurarea DNS, poți întâlni două formate de adrese: o adresă IP numerică (de exemplu, 94.140.14.14) sau un nume de gazdă (de exemplu, dns.adguard-dns.com). Acestea nu sunt același lucru — există o diferență fundamentală între ele.

**Adresa IP **se introduce în setările Wi-Fi sau Ethernet. Aceasta înseamnă că dispozitivul va trimite interogări DNS către serverul ales, dar fără criptare: interogările rămân deschise pentru observații externe. Este mai bine decât nimic, dar nu oferă o protecție completă.

**Numele gazdei (Hostname) **se introduce în câmpuri speciale: „DNS privat” pe Android, „DNS over HTTPS” în setările browserului, precum și în router. În acest caz, dispozitivul stabilește mai întâi o conexiune TLS securizată cu serverul și prin aceasta sunt transmise interogările — complet criptate.

* Pe scurt: Adresa IP în setările Wi-Fi înseamnă schimbarea serverului fără criptare. Numele gazdei în câmpul „DNS privat” sau în setările browserului înseamnă DNS securizat cu criptare completă. Dacă aveți de ales — alegeți a doua variantă.*

**Windows 10 și 11**

- Faceți clic dreapta pe pictograma rețelei din colțul din dreapta jos al ecranului.

- Selectați „Setări rețea și internet”.

- Faceți clic pe „Setări avansate ale plăcii de rețea” (în Windows 10 — „Modificare opțiuni adaptor”).

- Faceți clic dreapta pe conexiunea activă (Wi-Fi sau Ethernet) → „Proprietăți”.

- Selectați „Internet Protocol Version 4 (TCP/IPv4)” → faceți clic pe „Proprietăți”.

- Activați „Utilizează următoarele adrese de server DNS” și introduceți adresele IP ale serviciului ales.

- Faceți clic pe „OK” pentru a salva.

* Modificările vor intra în vigoare imediat — nu este necesară repornirea computerului.*

**macOS**

- Deschideți „Setări sistem” → „Rețea”.

- Selectați conexiunea activă din stânga → faceți clic pe „Detalii” (sau „Avansat”).

- Mergeți la fila „DNS”.

- Faceți clic pe „+” și introduceți adresa IP a serviciului, apoi repetați pentru a doua adresă.

- Faceți clic pe „OK” → „Aplicați”.

**Android**
Pe Android există două moduri de a schimba DNS-ul. Opțiunea „DNS privat” funcționează imediat pentru toate rețelele și utilizează criptarea — este varianta preferată.


- Deschideți „Setări” → „Conexiuni” (sau „Rețea și internet”).

- Căutați elementul „DNS privat” (poate fi în „Setări avansate”).

- Selectați „Nume gazdă furnizor DNS privat” și introduceți numele gazdei serviciului ales (vezi cardurile serviciilor de mai jos).

- Salvați modificările.

* Funcția „DNS privat” este disponibilă începând cu Android 9 (sau mai nou). Pe versiunile mai vechi, DNS-ul se schimbă separat pentru fiecare rețea Wi-Fi prin setările conexiunii, introducând adresele IP.*

**iPhone și iPad (iOS)**
iOS permite schimbarea DNS-ului separat pentru fiecare rețea Wi-Fi.


- Deschideți „Configurări” → „Wi-Fi”.

- Apăsați pe pictograma „ℹ️” de lângă numele rețelei curente.

- Derulați până la „Configurare DNS” și selectați „Manual”.

- Ștergeți adresele existente (apăsați pe „–” de lângă fiecare) și adăugați adresele IP ale serviciului ales.

- Apăsați pe „Salvați”.

* Setările trebuie repetate pentru fiecare rețea Wi-Fi. Internetul mobil (3G/4G/5G) utilizează DNS-ul operatorului.*

## Servicii DNS gratuite și de încredere

Toate serviciile enumerate mai jos acceptă criptarea și sunt disponibile gratuit. În setările Wi-Fi introduceți adresele IP: prima în câmpul „DNS principal”, a doua în câmpul „DNS secundar”. Pentru Android, utilizați numele gazdei în câmpul „DNS privat”.

**1. Google Public DNS**
*Jurisdicție: SUA (Alphabet Inc.). Politica de confidențialitate este disponibilă public.*

Google Public DNS este unul dintre cele mai răspândite servicii DNS publice din lume. Suportă verificarea autenticității prin DNSSEC, protocolul TLS 1.3 și protecția împotriva otrăvirii cache-ului. Datele despre interogări nu sunt stocate permanent.

**DNS principal: **8.8.8.8

**DNS secundar: **8.8.4.4

**2. Cloudflare DNS**
*Jurisdicție: SUA (Cloudflare Inc.). Servere în toată lumea. Politica de confidențialitate este disponibilă public.*

Cloudflare DNS criptează toate interogările prin DNS over HTTPS (DoH) și DNS over TLS (DoT). Garantează disponibilitate 100% datorită rețelei Anycast în peste 310 orașe. Adresele IP ale utilizatorilor nu sunt stocate, toate jurnalele sunt șterse în decurs de 24 de ore.

Cloudflare oferă, de asemenea, variante suplimentare sub numele 1.1.1.1 for Families — pentru familiile cu copii:


- 1.1.2 / 1.0.0.2 — blochează malware-ul și site-urile de phishing. Nume gazdă: **security.cloudflare-dns.com**

- 1.1.3 / 1.0.0.3 — blochează malware-ul, phishing-ul și conținutul pentru adulți. Nume gazdă: **family.cloudflare-dns.com**

**DNS principal: **1.1.1.1

**DNS secundar: **1.0.0.1

**Nume gazdă (Android): **one.one.one.one

**Aplicație (Android/iOS): **[1.1.1.1 + WARP](https://play.google.com/store/apps/details?id=com.cloudflare.onedotonedotonedotone)

**3. Quad9**
*Jurisdicție: Elveția (Quad9 — organizație non-profit). Acționează în cadrul legislației elvețiene.*

Quad9 blochează automat accesul la domeniile malițioase pe baza bazelor de date actuale de amenințări. Eficiența este de 97% împotriva domeniilor de malware și phishing. Nu păstrează jurnale cu date personale, funcționează în peste 200 de locații în peste 90 de țări.

Sunt disponibile trei variante de servere:


- 9.9.9.9 — serviciu securizat cu blocare malware și phishing, DNSSEC (recomandat)

- 9.9.10.10 — fără blocarea amenințărilor; doar pentru testare

- 9.9.11.11 — securizat cu suport EDNS Client Subnet (ECS)

**Nume gazdă (Android): **dns.quad9.net

**4. OpenDNS**
*Jurisdicție: SUA (Cisco Systems). Jurnalele sunt păstrate doar pentru scurt timp. Politica de confidențialitate este disponibilă public.*

OpenDNS protejează orice dispozitiv din rețea — de la computere și smartphone-uri la televizoare inteligente. Oferă protecție împotriva phishing-ului și malware-ului, control parental, filtrare personalizabilă a conținutului, blocarea reclamelor și a trackerelor.

**DNS principal: **208.67.222.222

**DNS secundar: **208.67.220.220

**5. NextDNS**
*Jurisdicție: Franța (NextDNS Inc.). Acționează în conformitate cu GDPR.*

NextDNS se remarcă prin posibilități extinse de configurare: filtrarea conținutului, blocarea reclamelor și a trackerelor, liste proprii de blocare și permisiune, DNSSEC, suport pentru toate platformele. Planul gratuit include 300.000 de interogări pe lună, un număr nelimitat de dispozitive și configurații.

**DNS principal: **45.90.28.232

**DNS secundar: **45.90.30.232

**6. Mullvad DNS**
*Jurisdicție: Suedia (Amagicom AB). Serviciul a trecut printr-un audit independent. Cod sursă deschis.*

Mullvad DNS este un serviciu DNS securizat gratuit oferit de compania suedeză de VPN Mullvad. Nu este necesară înregistrarea — serviciul este disponibil gratuit pentru oricine. Serverele rulează exclusiv în memoria RAM fără a scrie date pe disc. Sunt disponibile presetări:


- mullvad.net — doar criptare, fără blocare; IP: 194.242.2.2

- dns.mullvad.net — blochează reclamele și trackerele; IP: 194.242.2.3

- dns.mullvad.net — reclame, trackere și malware; IP: 194.242.2.4

- dns.mullvad.net — blochează suplimentar conținutul pentru adulți; IP: 194.242.2.6

* Mullvad DNS se configurează prin numele gazdei sau adresa IP — DNS-ul UDP/53 obișnuit nu este acceptat. Pe Android — prin „DNS privat”, pe iOS — printr-un profil de pe GitHub-ul companiei.*

## Ce serviciu să alegi

Toate cele șase servicii oferă un nivel de bază de protecție, iar alegerea între ele depinde de ceea ce este important pentru tine.

**Dacă vrei ceva simplu și fiabil **— Cloudflare (1.1.1.1) sau Google (8.8.8.8). Ambele servicii funcționează rapid, stabil și fără configurări suplimentare.

**Dacă este importantă protecția împotriva conținutului malițios **— Quad9 (9.9.9.9). Acest serviciu blochează automat site-urile de phishing și domeniile cu malware — acest lucru este deosebit de relevant pentru cei care doresc un nivel suplimentar de protecție fără nicio configurare.

**Dacă ai nevoie de setări flexibile: blocarea reclamelor, control parental, reguli proprii **— NextDNS sau Mullvad DNS. Ambele sunt servicii europene și oferă un control detaliat asupra filtrării.

Principalul lucru: oricare dintre aceste servicii este mai bun în ceea ce privește securitatea decât DNS-ul furnizorului tău de internet — iar configurarea durează doar câteva minute.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/6-bezkoshtovnyh-zahyshhenyh-dns-servisiv-yak-zashyfruvaty-svij-internet-trafik/?utm_source=responsabil) și a fost tradus în limba română.
