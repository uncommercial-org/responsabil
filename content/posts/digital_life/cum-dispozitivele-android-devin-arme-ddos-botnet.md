---
title: "Cum transformă atacatorii cibernetici dispozitivele Android în arme pentru atacuri DDoS: de la aplicații mobile la botneturi de milioane"
date: 2026-05-12
draft: false
description: "În 2025, botneturile Android precum Aisuru-Kimwolf și BadBox 2.0 stabilesc recorduri mondiale de atacuri DDoS. Descoperă cum gadgeturile ieftine și aplicațiile devin arme cibernetice."
categories: ["digital_life"]
tags: ["atacuri ddos", "securitate android", "botnet", "securitate cibernetică", "malware", "dispozitive mobile"]
cover:
  image: "images/cybercalm/cum-dispozitivele-android-devin-arme-ddos-botnet.webp"
  alt: "Ilustrație cu logo-ul Android și conexiuni digitale reprezentând o rețea botnet pentru atacuri DDoS."
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

În 2025, botneturile Android au devenit principala sursă a celor mai puternice atacuri DDoS din istoria internetului. Rețeaua Aisuru-Kimwolf, formată în principal din dispozitive smart TV box și dispozitive mobile cu Android, a stabilit în decembrie un record mondial — 31,4 Tbps. O altă amenințare, BadBox 2.0, a cuprins peste 10 milioane de dispozitive care sunt vândute efectiv cu un backdoor ascuns. Vă explicăm cum aplicațiile malițioase și gadgeturile Android ieftine transformă locuințele a milioane de oameni în noduri ale infrastructurii globale de atacuri cibernetice.

În urmă cu cinci ani, atacurile DDoS de pe dispozitivele mobile erau considerate un fenomen rar. În mai 2020, cercetătorii ESET [au publicat o analiză](https://www.welivesecurity.com/2020/05/11/breaking-news-app-promises-news-brings-ddos-attacks/) a aplicației 'Updates for Android', care se masca sub forma unui flux zilnic de știri în Google Play. Programul a adunat peste 50.000 de descărcări și, la comanda unui server la distanță, a început să genereze trafic împotriva site-ului ESET. Atacul a durat șapte ore, implicând aproximativ 4.000 de adrese IP unice.

Atunci, acesta părea un incident atipic — iar expertul ESET Lukáš Štefanko spunea direct că atacatorii și-au "dezvăluit botnetul degeaba", deoarece instrumentul a încetat să mai existe după ce Google a eliminat aplicația din magazin. Astăzi, această poveste se citește diferit: a fost un semnal timpuriu a ceea ce urma să devină vectorul dominant în industria globală DDoS.

## **Ce s-a schimbat în cinci ani: botneturile Android au trecut în prim-plan**

Conform [raportului trimestrial Cloudflare despre DDoS](https://blog.cloudflare.com/ddos-threat-report-2025-q4/) pentru trimestrul patru din 2025, numărul total de atacuri DDoS la nivel mondial a crescut cu 121% de la an la an, ajungând la 47,1 milioane. Numărul atacurilor cu o putere de peste 100 de milioane de pachete pe secundă a crescut cu 600%, iar atacurile care depășesc 1 Tbps au crescut cu 65% pe trimestru. Majoritatea declanșatorilor sunt rafale scurte, care durează mai puțin de zece minute și reușesc să scoată din funcțiune infrastructura mai repede decât pot reacționa sistemele tradiționale de protecție.

Rolul cheie în această escaladare îl joacă tocmai botneturile mobile — rețele de dispozitive Android infectate. Dacă în 2020 vorbeam despre zeci de mii de smartphone-uri, astăzi este vorba despre milioane de dispozitive simultan, în special smart TV box-uri ieftine, proiectoare și alte gadgeturi bazate pe Android Open Source Project.

## **Aisuru-Kimwolf: botnetul care doboară recorduri de putere**

Aisuru-Kimwolf este cea mai puternică rețea DDoS de astăzi, construită în principal din dispozitive Android. Conform estimărilor Cloudflare, aceasta numără între 1 și 4 milioane de gazde infectate — majoritatea smart TV box-uri, streamere Android și dispozitive mobile. Kimwolf în sine este varianta pentru Android a botnetului "mamă" Aisuru, specializat în infectarea ecosistemului Android. Acesta are aproximativ 2 milioane de dispozitive, cu cea mai mare concentrație de infecții în Vietnam, Brazilia, India și Arabia Saudită.

În noaptea de 19 decembrie 2025, operatorii Aisuru au desfășurat o campanie pe care Cloudflare a numit-o "The Night Before Christmas". Vârful său a atins **31,4 Tbps** — acesta fiind cel mai mare atac DDoS înregistrat public din istorie. În paralel, au avut loc atacuri HTTP cu o putere de peste 200 de milioane de cereri pe secundă. Cu trei luni înainte, aceeași rețea stabilise recordul de atunci de 29,7 Tbps, iar într-un singur trimestru din 2025, Cloudflare a blocat 1.304 atacuri hiper-volumetrice de la Aisuru — în medie 14 pe zi.

Pericolul deosebit al Aisuru-Kimwolf constă nu doar în amploare, ci și în modelul de monetizare. Operatorii vând "bucăți" din botnet ca serviciu prin canale de Telegram și Discord. Un atac la scară națională, capabil să scoată din funcțiune rețelele magistrale sau furnizorii de internet ai unei țări întregi, costă cumpărătorul de la câteva sute la câteva mii de dolari SUA. Dispozitivele infectate sunt folosite și ca proxy-uri rezidențiale — operatorii închiriază adresele lor IP pentru a masca alte atacuri cibernetice, scraping de date sau brute-forcing de conturi.

Kimwolf se răspândește în principal prin interfețele deschise Android Debug Bridge (ADB) și infrastructura de proxy-uri rezidențiale. Conform datelor Synthient, săptămânal sunt înregistrate aproximativ 12 milioane de adrese IP unice din acest botnet.

## **BadBox 2.0: când dispozitivul este deja infectat în magazin**

A doua mare amenințare mobilă din 2025 este botnetul BadBox 2.0. În iunie, FBI a emis un [avertisment public](https://www.ic3.gov/PSA/2025/PSA250605) conform căruia milioane de dispozitive IoT de uz casnic conectate la rețelele domestice sunt compromise de acest software malițios. Este vorba despre TV box-uri ieftine, proiectoare digitale, rame foto, sisteme de infotainment auto și tablete — în principal dispozitive fără brand cu Android Open Source Project, fabricate în China continentală.

Caracteristica fundamentală a BadBox 2.0 este că dispozitivele sunt infectate *chiar înainte ca cumpărătorul să le scoată din cutie*. Software-ul malițios este fie deja integrat în firmware în etapa de producție, fie se instalează în timpul primei configurări — când dispozitivul descarcă aplicații "obligatorii" cu backdoor-uri. A doua strategie de infectare sunt aplicațiile false "clonă" din magazine neoficiale, care imită software-ul popular. Utilizatorilor li se cere adesea să dezactiveze Google Play Protect pentru a instala acces "gratuit" la conținut.

În iulie 2025, Google [a depus o plângere](https://krebsonsecurity.com/2026/01/who-operates-the-badbox-2-0-botnet/) la tribunalul federal din New York împotriva a 25 de persoane neidentificate care se află în spatele BadBox 2.0. În documentele instanței, compania descrie botnetul ca fiind "cea mai mare rețea cunoscută de dispozitive smart TV compromise", cu peste 10 milioane de dispozitive. Într-o operațiune comună a Google, HUMAN Security, Trend Micro și Shadowserver Foundation, s-a reușit deconectarea a peste 500.000 de dispozitive infectate de la serverele de control. Totuși, cercetătorii avertizează: este imposibilă demontarea completă a infrastructurii, deoarece lanțul de aprovizionare cu dispozitive infectate din China continuă să funcționeze.

Cele mai mari concentrații de infecții BadBox 2.0 sunt în Brazilia (37,6%), SUA (18,2%), Mexic (6,3%) și Argentina (5,3%). În total, botnetul a cuprins 222 de țări. Printre modelele cel mai des identificate ca fiind compromise se numără TV box-urile TV98, GameBox și o întreagă serie de alte dispozitive fără brand care nu sunt certificate de Google Play Protect.

## **Cum anume se transformă aplicațiile mobile într-un instrument DDoS**

Schema tehnică descrisă de ESET în 2020 pe exemplul 'Updates for Android' nu s-a schimbat în esență — doar s-a scalat. Scenariul constă în câțiva pași:

*   **Etapa aplicației 'curate'.** Atacatorii publică o aplicație fără funcții malițioase — pentru a trece moderarea magazinului și a strânge o bază de utilizatori. În cazul 'Updates for Android', au trecut aproximativ patru luni până la adăugarea codului malițios.
*   **Activarea prin actualizare.** Când baza de instalări devine suficient de mare, apare o actualizare cu un modul care primește comenzi de la serverul de comandă (C&C). În vechiul caz ESET, aplicația contacta serverul la fiecare 150 de minute și transmitea identificatorul dispozitivului.
*   **Descărcarea JavaScript.** Serverul livrează un script cu domeniul țintă, după care dispozitivul începe să trimită cereri către acest domeniu cu o frecvență de aproximativ una pe secundă — până la primirea unei noi comenzi.
*   **Mascare.** Aceeași tehnică de execuție la distanță a JavaScript este utilizată de zeci de framework-uri Android legitime, motiv pentru care detectarea automată dă multe rezultate fals pozitive. Acesta rămâne unul dintre motivele pentru care astfel de aplicații ajung în Google Play.

În botneturile moderne, cum ar fi Aisuru-Kimwolf, la această schemă s-au adăugat exploatarea serviciilor deschise ADB, funcționalitatea de proxy pentru rutarea traficului terț, posibilitatea de a descărca și executa fișiere APK arbitrare, precum și module pentru interceptarea codurilor de autentificare în doi pași și reclame.

## **Cum să vă protejați: ce puteți face chiar astăzi**

Amenințarea vizează în principal dispozitivele ieftine, fără brand, bazate pe Android Open Source Project — smartphone-uri necertificate de Google Play Protect din surse dubioase și, mai ales, TV box-uri vândute ca fiind "deblocate" pentru vizionarea gratuită a serviciilor de streaming. FBI și cercetătorii în securitate recomandă următorii pași:

*   **Cumpărați doar dispozitive certificate.** Înainte de achiziție, verificați dacă dispozitivul are certificarea Google Play Protect. TV box-urile fără brand, promovate ca fiind "deblocate" sau "cu acces gratuit la servicii plătite", reprezintă principalul grup de risc.
*   **Nu dezactivați Google Play Protect.** Dacă o aplicație cere dezactivarea acestei funcții, acesta este un semnal de alarmă. Play Protect avertizează și blochează automat programele cu comportament cunoscut de BadBox 2.0.
*   **Descărcați aplicații doar din magazinele oficiale.** Evitați fișierele APK terțe și marketplace-urile neoficiale — prin acestea se răspândesc 'aplicațiile clonă' cu backdoor-uri.
*   **Urmăriți permisiunile.** Verificați ce drepturi solicită programul și dacă acestea corespund scopului său declarat. O aplicație de tip flux de știri nu are nevoie de acces la conexiuni de rețea în fundal sau de permisiunea de a afișa reclame peste alte programe.
*   **Monitorizați traficul de rețea.** Semne suspecte ale unui dispozitiv infectat: trafic de ieșire inexplicabil, descărcarea rapidă a bateriei, supraîncălzirea, apariția unor aplicații necunoscute, consum neașteptat de date mobile.
*   **Actualizați firmware-ul și sistemul de operare.** Actualizările regulate închid vulnerabilitățile cunoscute prin care se răspândește Kimwolf — în special interfețele ADB deschise.
*   **Deconectați dispozitivele suspecte de la rețeaua domestică.** Dacă există suspiciunea că un TV box sau un alt gadget IoT este compromis, FBI recomandă scoaterea imediată a acestuia din rețea.

Separat, merită reținut: antivirușii de origine rusă (Kaspersky, Dr.Web) nu sunt recomandați pentru utilizare în Ucraina. Pentru protecția dispozitivelor mobile, ar trebui alese soluții ale dezvoltatorilor europeni, americani sau ucraineni.

## **Ce concluzii tragem**

Povestea 'Updates for Android' din 2020 arată astăzi ca o uvertură. Atunci, 50.000 de smartphone-uri infectate și un atac asupra ESET păreau o excepție. În 2025, botneturile formate din dispozitive Android au devenit instrumentul principal al cibercriminalilor pentru atacuri hiper-volumetrice — iar accesul la acestea se vinde pe piața neagră ca un serviciu obișnuit. Acest lucru înseamnă că chiar și o organizație mică poate deveni astăzi ținta unui atac de câțiva terabiți pe secundă, comandat pentru o mie de dolari.

Pentru utilizatorul obișnuit, concluzia este simplă: un gadget Android ieftin și fără brand nu reprezintă doar un risc pentru proprietar, ci și o contribuție la infrastructura globală de atacuri. Verificați certificarea dispozitivelor înainte de cumpărare, nu dezactivați Play Protect, nu instalați aplicații din surse nesigure — iar acest lucru elimină deja cea mai mare parte a riscului individual.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/yak-kiberzlochyntsi-vykorystovuyut-mobilni-dodatky-dlya-ddos-atak/?utm_source=responsabil) și a fost tradus în limba română.
