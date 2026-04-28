---
title: "Cum interacționează infractorii cibernetici între ei"
date: 2026-04-21
draft: false
description: "O privire detaliată asupra ecosistemului criminalității cibernetice: de la brokeri de acces la modelele de tip „as-a-service” și rolul AI sau Telegram în atacurile moderne."
categories: ["securitate"]
cover:
  image: "images/cybercalm/cum-interactioneaza-infractorii-cibernetici-intre-ei.webp"
  alt: ""
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

În rapoartele de securitate cibernetică, este obișnuit ca atacurile hackerilor să fie descrise ca evenimente izolate — dar, în realitate, în spatele fiecărei breșe de succes se află o întreagă rețea de furnizori de servicii, intermediari și executanți interdependenți. Criminalitatea cibernetică a încetat de mult să fie apanajul singuraticilor și s-a transformat într-o industrie subterană în toată regula, cu propria piață a forței de muncă, lanțuri de aprovizionare și chiar concurență între „vânzători”.

Potrivit estimărilor cercetătorilor, în 2025, pierderile globale cauzate de criminalitatea cibernetică au ajuns la 10,5 trilioane de dolari pe an — mai mult decât PIB-ul oricărei țări din lume, cu excepția SUA și a Chinei. Pentru comparație: aceasta depășește de două ori PIB-ul Ucrainei din întreaga sa istorie de independență, luată împreună. Criminalitatea cibernetică sub formă de model de servicii a făcut atacurile accesibile chiar și persoanelor fără cunoștințe tehnice: achiziționarea unui instrument gata făcut pentru hacking este la fel de ușoară ca și comandarea livrării de mâncare.

Compania de securitate cibernetică [CrowdStrike](https://www.crowdstrike.com/) a sistematizat acest ecosistem încă din 2021, împărțindu-l în trei categorii mari: servicii, distribuție și monetizare. Astăzi, această structură rămâne relevantă, dar fiecare dintre categorii a evoluat semnificativ — și a fost completată de două dimensiuni noi, care nu existau acum cinci ani: inteligența artificială și Telegram ca principală platformă de comerț subteran.

## Nivelul unu: servicii și furnizori

Infrastructura de bază a criminalității cibernetice este un set de servicii specializate pe care grupurile infracționale le „închiriază” sau le cumpără în loc să le dezvolte singure. Principiul este același ca în afacerile tehnologice legale: de ce să construiești propriul centru de date dacă poți închiria un cloud?

### Brokerii de acces inițial (Initial Access Brokers)

Aceasta este, probabil, cea mai vizibilă categorie a pieței subterane din ultimii ani. Brokerii de acces sunt atacatori specializați în spargerea rețelelor corporative și vânzarea ulterioară a acestui acces către alte grupuri. Ei nu efectuează atacurile singuri — ei furnizează „ușa deschisă”.

Conform datelor Group-IB, în 2024 au fost înregistrate peste 3.000 de oferte de vânzare a accesului la rețelele corporative — cu 15% mai mult față de 2023. Regiunea Americii de Nord a înregistrat cea mai mare creștere — 43%. Prețurile variază de la câteva sute la zeci de mii de dolari, în funcție de mărimea organizației și nivelul de privilegii.

### Ransomware-as-a-Service și Crime-as-a-Service

Modelul „ransomware ca serviciu” (RaaS) a democratizat practic unul dintre cele mai profitabile tipuri de criminalitate cibernetică. Dezvoltatorii de programe ransomware nu mai efectuează atacurile singuri — ei creează platforma și vând sau închiriază accesul la aceasta către afiliați, primind între 10% și 30% din fiecare răscumpărare plătită.

În 2024, Group-IB a identificat 39 de noi anunțuri RaaS și a înregistrat o creștere de 44% a numărului de afiliați. Numărul atacurilor prin intermediul site-urilor specializate de scurgeri de date a crescut cu 10% — la peste 5.000 de cazuri documentate. În 2024, o companie din lista Fortune 50 a plătit o răscumpărare record de 75 de milioane de dolari.

### Servicii de anonimizare și găzduire „bulletproof”

Infrastructura de anonimat este un alt element cheie al pieței subterane. Aceasta include rețele proxy rezidențiale (traficul este direcționat prin dispozitivele utilizatorilor reali, ceea ce îl face aproape nedetectabil), servicii VPN private fără jurnale de activitate, precum și furnizori de găzduire „bulletproof” — companii care oferă infrastructură de servere și ignoră în mod deliberat reclamațiile privind abuzurile.

### Kituri de phishing și Webinject

Kiturile de phishing — instrumente web gata făcute pentru automatizarea atacurilor de phishing — sunt disponibile pe piețele subterane pentru sume începând de la câteva zeci de dolari. Instrumente mai complexe de tip Webinject permit injectarea codului malițios direct în browser-ul victimei în timp ce aceasta vizitează site-uri bancare — victima vede interfața obișnuită, dar în realitate interacționează cu un strat malițios.

### Servicii de recrutare și „carăușii de bani” (money mules)

Recrutarea oamenilor obișnuiți pentru a participa la scheme infracționale este o specializare separată. Așa-numiții „carăuși de bani” retrag fizic numerar din conturile compromise sau primesc transferuri în contul propriu, trimitând apoi fondurile mai departe pe lanțul de spălare a banilor. O parte din acești oameni sunt recrutați conștient pe forumuri subterane; alții devin victime ale escrocilor care promit „câștiguri ușoare”.

## Nivelul doi: distribuția și livrarea atacurilor

Chiar și cel mai sofisticat software malițios este inutil fără un mecanism de livrare. De aceea, distribuția este un segment separat al pieței subterane, cu proprii specialiști și servicii.

**Campaniile de spam și phishing** rămân cel mai răspândit instrument de infiltrare inițială. Conform datelor ENISA, phishing-ul este vectorul dominant de atac în 60% din incidentele documentate în Uniunea Europeană. Anumite grupuri se specializează exclusiv în trimiteri masive — ei nu dezvoltă malware și nu monetizează datele, „produsul” lor fiind acoperirea audienței.

O altă categorie cheie sunt **„loader-ele”**. Acestea sunt grupări care controlează deja dispozitive infectate și oferă servicii de „instalare” a software-ului malițios al altui grup într-o rețea deja compromisă. Practic, este un serviciu de subcontractare: un grup construiește capul de pod, altul îl folosește pentru propriile scopuri.

**Exploit kits** — seturi pentru exploatarea automată a vulnerabilităților în browsere și plugin-uri — permit infectarea dispozitivelor victimelor fără nicio interacțiune din partea acestora: este suficientă simpla vizitare a unui site compromis. Traficul către astfel de site-uri este redirecționat prin resurse web legitime compromise, ceea ce complică detectarea.

## Nivelul trei: monetizarea — transformarea spargerii în bani

Spargerea unei rețele este doar jumătate din treabă. Următoarea sarcină este convertirea datelor obținute sau a accesului în bani reali, rămânând în același timp nedetectat. Monetizarea este cel mai divers segment al ecosistemului criminalității cibernetice.

**Forumurile de carding** rămân piața principală de desfacere pentru datele de plată furate. Prețul depinde de tipul cardului, țară și disponibilitatea „dump-ului” complet cu codul CVV. Servicii separate de verificare a cardurilor permit verificarea automată a valabilității a mii de numere în câteva minute.

Spălarea banilor a evoluat odată cu criptomonedele. **„Mixerele” și „tumbler-ele”** — servicii care amestecă tranzacțiile cripto pentru a ascunde originea lor — au devenit un instrument standard. Conform datelor Chainalysis, volumul total al criminalității cripto în 2024 a depășit 51 de miliarde de dolari. În paralel, există rețele de companii-fantomă pentru spălarea fondurilor prin canale bancare legale.

**„Revânzarea frauduloasă”** — o schemă prin care fondurile furate sunt convertite în bunuri reale (de obicei electronice, bijuterii sau mașini), care sunt apoi revândute pe numerar. Acest lucru complică urmărirea: banii sunt „curățați” prin piața legală de mărfuri.

Șantajul este o altă formă de monetizare care a depășit cu mult limitele ransomware-ului clasic. Astăzi, este răspândit **„atacul dublu”**: criptarea datelor și, simultan, amenințarea cu publicarea acestora. Unele grupări au renunțat complet la criptare și se ocupă exclusiv de furt și șantaj — este mai simplu și la fel de profitabil.

## O nouă dimensiune: inteligența artificială ca amplificator al criminalității

Acum cinci ani, AI în criminalitatea cibernetică era o raritate. Astăzi, este integrată în ecosistemul subteran ca un instrument standard. Cercetătorii de la Trend Micro au observat o schimbare fundamentală: infractorii nu mai construiesc singuri instrumente AI — ei cumpără servicii gata făcute sau sparg platforme legale.

**Jailbreak-as-a-Service** este un segment separat de piață: furnizorii vând metode de ocolire a protecției modelelor lingvistice comerciale (ChatGPT, Claude, Gemini) pentru generarea de e-mailuri de phishing, scenarii de inginerie socială și cod malițios. Pe piețele subterane se vând, de asemenea, conturi compromise de ChatGPT și Claude — pentru automatizare masivă sau ocolirea sancțiunilor (relevant pentru Rusia, Iran și Coreea de Nord, unde accesul la aceste servicii este blocat).

**Tehnologiile deepfake** s-au transformat dintr-o curiozitate într-un instrument de fraudă corporativă. Au fost înregistrate cazuri în care atacatorii au falsificat mesaje video și audio ale conducătorilor de companii pentru a forța angajații de la departamentul financiar să efectueze transferuri mari. Evaluarea amenințărilor Europol pentru 2025 avertizează direct: grupările infracționale utilizează tot mai activ AI generativ pentru scalarea phishing-ului și a operațiunilor de fraudă.

În paralel, apar primele mostre de malware care generează dinamic propriul cod cu ajutorul modelelor lingvistice încorporate — adaptându-se la mediul specific și complicând detectarea. Deocamdată, aceste tehnici rămân de nișă din cauza instabilității și dependenței de API-uri externe, dar tendința a fost înregistrată.

## Noua infrastructură: Telegram a înlocuit darknet-ul

Dacă acum cinci ani principala platformă de comerț subteran erau forumurile anonime din rețeaua Tor și piețele darknet, astăzi centrul de greutate s-a mutat către Telegram. Un studiu al companiei Cyfirma confirmă: Telegram a devenit principala platformă pentru hackeri.

Amploarea este impresionantă. Numai printr-un singur grup din Telegram — Huione Guarantee — din 2021 până în 2025 au trecut tranzacții în valoare de 27 de miliarde de dolari legate de activități ilegale. Aceasta depășește cifra de afaceri a celor mai cunoscute piețe darknet din întreaga lor istorie. Când în mai 2025 Telegram a blocat acest canal, locul său a fost ocupat instantaneu de clone — și în doar câteva luni, noul canal a atins o cifră de afaceri de 1,1 miliarde de dolari.

Telegram îi atrage pe infractori din mai multe motive: anonimat relativ, posibilitatea de a crea grupuri închise mari, integrare facilă cu boți de criptomonede și o complexitate tehnică mult mai mică față de Tor. Vânzarea bazelor de date compromise, a cardurilor de credit, a instrumentelor de hacking, recrutarea „carăușilor de bani” — toate acestea au loc în canale deschise și închise cu o moderare minimă.

*După arestarea lui Pavel Durov în Franța în august 2024, Telegram a anunțat transferul către autoritățile de aplicare a legii a datelor utilizatorilor implicați în activități ilegale. În 2024, platforma a blocat peste 15,3 milioane de canale și grupuri. Cu toate acestea, conform observațiilor cercetătorilor, activitatea infracțională cibernetică pe Telegram continuă să crească.*

## De ce vizarea furnizorilor este mai eficientă decât urmărirea executanților

Urmărirea tuturor legăturilor dintre grupări și furnizorii acestora este o sarcină extrem de dificilă din cauza utilizării pe scară largă a canalelor de comunicare criptate și a criptomonedelor. Totuși, compania de analiză Chainalysis a formulat încă din 2021 un principiu care rămâne relevant: organele de drept obțin rezultate mai bune dacă atacă infrastructura comună, nu executanții finali.

Logica este simplă: distrugerea unui serviciu RaaS înseamnă scoaterea simultană din funcțiune a zeci de grupări care îl foloseau. Spargerea unei rețele de găzduire „bulletproof” înseamnă privarea de infrastructură a unui întreg cluster de operațiuni criminale. Această abordare a arătat rezultate reale: operațiunile împotriva infrastructurii Emotet (2024) și ALPHV/BlackCat (2024) au cauzat daune mult mai mari ecosistemului criminal decât arestările punctuale ale unor hackeri individuali.

Există și un alt avantaj: furnizorii de servicii subterane au, de obicei, o securitate operațională mai slabă decât cele mai mari grupări infracționale. „Urmele” lor rămân în datele care ajută ulterior la identificarea clienților de nivel superior.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/yak-kiberzlochyntsi-vzayemodiyut-mizh-soboyu/?utm_source=responsabil) și a fost tradus în limba română.
