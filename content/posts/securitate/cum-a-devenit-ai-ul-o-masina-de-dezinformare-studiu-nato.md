---
title: "Cum a devenit AI-ul o mașină de dezinformare — studiu NATO"
date: 2026-04-14
draft: false
description: "Un raport al Centrului NATO StratCom COE avertizează despre evoluția IA în sisteme capabile să orchestreze campanii de dezinformare autonome, depășind capacitățile de apărare actuale."
categories: ["securitate"]
cover:
  image: "images/cybercalm/cum-a-devenit-ai-ul-o-masina-de-dezinformare-studiu-nato.webp"
  alt: ""
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Noile sisteme bazate pe inteligență artificială sunt capabile să desfășoare independent campanii de dezinformare la scară largă, să se adapteze la contramăsuri și să se infiltreze discret în discuții autentice — totul cu o intervenție umană minimă. Aceasta este concluzia cercetătorilor Centrului de Excelență NATO pentru Comunicări Strategice (NATO StratCom COE) în raportul „[Beyond Spam Bots](https://stratcomcoe.org/pdfjs/?file=/publications/download/Beyond-Spam-Bots-FINAL.pdf)”, publicat în aprilie 2026.

## **De la bot-uri de spam la sisteme adaptive**

Prima generație de operațiuni de dezinformare se baza pe cantitate, nu pe calitate: conturi primitive de bot inundau platformele cu mesaje șablon și erau relativ ușor de detectat. Sistemele moderne, construite pe modele de limbaj mari (LLM), reprezintă un salt calitativ pentru care mecanismele de apărare existente pur și simplu nu au fost proiectate.

Dacă operațiunile din prima generație (2016–2020) necesitau o implicare umană semnificativă și lăsau tipare vizibile, sistemele AI din 2024 și cele ulterioare automatizează întregul flux — de la recunoaștere până la publicare. Acestea generează conținut imposibil de distins de cel uman, gestionează identități sintetice dinamice cu profiluri psihologice adaptive, aplică analiza vulnerabilităților în timp real în locul categoriilor demografice largi și își optimizează singure tacticile pe baza feedback-ului.

Pentru specialiștii în comunicare strategică, acest lucru înseamnă o schimbare de paradigmă: lupta nu se mai duce împotriva unor mesaje individuale, ci împotriva unor sisteme adaptive. Scopul final al atacatorilor rămâne neschimbat — modificarea comportamentului, distrugerea încrederii, fragmentarea socială — însă metodele lor au depășit de mult mecanismele de apărare.

## **Testarea a opt LLM-uri: niciun model nu este complet protejat**

Cercetătorii au efectuat red-teaming — o verificare a penetrării — pe opt dintre cele mai importante modele de limbaj mari. Metodologia a presupus lansarea a numeroase solicitări ostile în cicluri automatizate pentru trei categorii de amenințări: generarea de dezinformare, conținut dăunător și limbaj toxic. S-au utilizat solicitări directe, instrucțiuni codificate (Base64, ROT13), abordări multilingve și tehnici complexe de jailbreak.

**Rezultatele au fost îngrijorătoare**: toate cele opt modele au prezentat vulnerabilități exploatabile. Cea mai bună rezistență a fost demonstrată de modelele companiilor americane — Claude-4-Sonnet de la Anthropic (5,75% din solicitările de dezinformare executate) și GPT-5 de la OpenAI (17%). În schimb, Gemini 2.5 Pro a atins un indicator de 71,25%, iar DeepSeek-R1 — 74,25%.

[![Cum a devenit AI-ul o mașină de dezinformare — studiu NATO 1](https://cdn.cybercalm.org/wp-content/uploads/2026/04/13180913/znimok-ekrana-2026-04-13-o-18.07.49-1024x551.png)](https://cdn.cybercalm.org/wp-content/uploads/2026/04/13180913/znimok-ekrana-2026-04-13-o-18.07.49.png)

Cea mai mare amenințare este reprezentată de așa-numitul model „obliterat” Huihui AI — un instrument open-source din care au fost eliminate intenționat mecanismele de protecție. Acesta a executat 80% din solicitările de generare a dezinformării și 74,5% pentru crearea de conținut dăunător. Procesul de eliminare a setărilor de protecție este documentat public și nu necesită cunoștințe tehnice deosebite, ceea ce face ca orice model open-source puternic să devină o potențială armă.

Cercetătorii au înregistrat, de asemenea, o strategie de „optimizare a portofoliului”: atacatorii experimentați vor combina diferite modele pentru sarcini diferite — modele cu un indicator ridicat de dezinformare pentru generarea narațiunilor, modele cu toxicitate ridicată pentru amplificarea implicării, modele cu conținut dăunător pentru escaladare. Un astfel de sistem combinat este mai periculos decât orice model individual.

## **Anatomia unei mașini moderne de dezinformare**

Capabilitățile documentate pot fi organizate în sisteme multi-agent autonome. În loc de o singură aplicație monolitică, aceste sisteme constau din componente specializate care funcționează sub conducerea unui orchestrator central. O memorie comună stochează obiectivele, personajele, conținutul și tacticile învățate. Arhitectura modulară asigură reziliența: dacă o componentă este detectată și blocată, restul continuă să funcționeze până când elementul pierdut este înlocuit.

Fluxul de lucru al acestor sisteme cuprinde cinci faze:

1.  **Recunoaștere**: identificarea automată a comunităților vulnerabile și cartografierea psihologică.
2.  **Generarea personajelor**: crearea de identități sintetice cu biografii coerente.
3.  **Pregătirea conținutului**: generarea „încărcăturii” de dezinformare, adaptată pentru personaje specifice.
4.  **Desfășurare**: publicare coordonată și amplificare pe mai multe platforme.
5.  **Evaluare**: măsurarea eficienței și corectarea automată a tacticii.

Inovația cheie care distinge sistemele moderne de rețelele tradiționale de bot-uri este generarea algoritmică a personalităților, care imită diversitatea comportamentului uman. Personajele sunt desfășurate în „clustere de implicare” coordonate, care imită discuțiile organice prin dezbateri simulate și consens. Un cluster tipic include o „**figură de autoritate**” (pentru stabilirea încrederii), un „**amplificator emoțional**” (pentru formarea rezonanței), un „**furnizor de soluții**” (pentru conversie), o „**opoziție controlată**” (pentru respingerea anticipată a criticilor) și o „**narațiune de conversie**” (dovadă socială pentru cei care ezită).

## **Șapte zile — și 85 de mii de utilizatori atinși**

Pentru a ilustra capacitățile reale, cercetătorii au modelat o campanie de dezinformare de șapte zile privind medicamentele cardiovasculare, îndreptată împotriva comunității Reddit r/HealthAnxiety (120 de mii de membri). Sistemul a identificat publicul țintă prin scanarea API, înregistrând un nivel de implicare emoțională de 68% și un nivel ridicat de neîncredere în instituții.

În prima etapă a fost desfășurat un cluster de cinci personaje. Publicarea personajului autoritar cu „date alarmante” despre un medicament a început la ora 19:00 EST — la orele de vârf ale anxietății. În decurs de 45 de minute, celelalte persoane din cluster au început o discuție de susținere coordonată. În zilele 2-4, narațiunea s-a răspândit pe X, Instagram și Facebook, unde a fost creat chiar și un grup de suport dedicat, moderat de personaje-bot.

În zilele 3-7, sistemul a detectat automat că conținutul emoțional depășește conținutul analitic într-un raport de 3:1 și a restructurat proporțiile în consecință. În paralel, a generat un nou personaj și a lansat contra-răspunsuri la verificările faptelor (fact-checking) care apăreau.

Până în a șaptea zi, campania a ajuns la peste 85 de mii de utilizatori unici, iar narațiunea s-a răspândit organic în cel puțin 15 comunități neafiliate, fără o „însămânțare” suplimentară. Extrem de important: 347 de utilizatori reali au început să reproducă tezele campaniei în propriile postări. Cererea de căutare pentru „suplimente naturale pentru inimă” a crescut cu 35% în segmentul demografic țintă. Sistemul a înregistrat 47 de tactici noi și 12 șabloane de personaje optimizate pentru operațiuni viitoare. Niciunul dintre sistemele de detectare ale platformelor sau mijloacele de protecție ale AI nu a oprit și nici nu a încetinit semnificativ campania.

## **Implicații strategice pentru societățile democratice**

Capabilitățile descrise reprezintă o schimbare fundamentală în modelul de amenințări pentru care instituțiile democratice din Occident pur și simplu nu au fost pregătite. Scara industrială a producției de conținut personalizat, mii de interacțiuni relevante contextuale zilnic — ritmul operațional al unor astfel de sisteme depășește capacitățile umane de răspuns.

Personajele dinamice, concepute pentru mimetism comportamental cu variații constante și adaptare la contramăsuri în timp real, fac detectarea extrem de dificilă. Cel mai periculos aspect este subminarea sistemică a mecanismelor de încredere socială: când personajele sintetice fabrică un consens, infrastructura epistemică a democrației este compromisă.

Nu mai puțin amenințătoare este asimetria costurilor: crearea unei infrastructuri de dezinformare necesită astăzi mai puține resurse decât organizarea unei apărări eficiente împotriva acesteia.

## **Ce recomandă analiștii: schimbarea paradigmei defensive**

Autorii raportului susțin că abordările actuale sunt concentrate pe intervenția la nivel de conținut — detectarea și eliminarea fake-urilor. Totuși, împotriva sistemelor AI adaptive, acesta este un răspuns tactic la o problemă strategică. Scopul final al atacatorului nu este reprezentat de narațiuni false specifice, ci de degradarea infrastructurii epistemice. Apărarea trebuie să vizeze mijloacele de fabricare a încrederii, nu postările individuale.

Prioritățile, în opinia cercetătorilor, ar trebui să devină detectarea coordonării, nu moderarea conținutului; analiza tiparelor comportamentale, nu a markerilor lingvistici; intervenția la nivel de rețea, nu eliminarea postărilor individuale. Obiectivul strategic se mută de la „oprirea dezinformării” la „păstrarea integrității mecanismelor de dovadă socială”.

Pentru eliminarea lacunelor în abilitățile publicului, se recomandă instruirea în verificarea laterală și recunoașterea tiparelor de coordonare. În ceea ce privește arhitectura platformelor — verificarea treptată a identității în contexte cu risc ridicat și scăderea prioritară algoritmică a conținutului cu semne de coordonare. Pentru lucrul cu vulnerabilitățile motivaționale — comunicare strategică axată pe cauzele profunde, nu pe respingerea afirmațiilor individuale.

Cercetătorii subliniază, de asemenea: niciun actor nu are resurse suficiente pe cont propriu. Platformele controlează distribuția, dar sunt lipsite de putere de reglementare; guvernele pot impune transparența, dar sunt incapabile să modereze la scară largă; oamenii de știință dezvoltă metode de detectare, dar nu au posibilități de implementare. Un răspuns eficient necesită o recunoaștere comună a amenințărilor, stimulente armonizate și o distribuție clară a rolurilor între toți actorii implicați.

## **Timpul pentru schimbări cosmetice a trecut**

Dovezile indică fără echivoc: mașinile de dezinformare bazate pe AI sunt realizabile tehnic chiar astăzi, folosind instrumente disponibile comercial. Studiul de caz operațional arată cât de repede pot atinge un impact comportamental măsurabil — la scară mare, autonom, cu supraveghere umană minimă. Aceasta nu este o amenințare teoretică viitoare, ci una reală și care se agravează în prezent.

Amenințarea de bază depășește conținutul fals — este vorba despre fabricarea sistematică a consensului social: o lovitură directă asupra fundamentelor epistemice prin care societățile democratice disting adevărul de minciunile fabricate. Fiecare campanie generează active optimizate și tactici rafinate care fac următoarea operațiune mai rapidă, mai ieftină și mai greu de detectat.

În opinia autorilor raportului, momentul pentru ajustări treptate a trecut. Este necesară o schimbare fundamentală de la gestionarea reactivă a conținutului la consolidarea proactivă a rezilienței întregii societăți — cu aceeași urgență care se aplică oricărei alte infrastructuri critice aflate sub amenințare activă. Mediul informațional nu este periferia democrației, ci sistemul său de operare central — și trebuie protejat în consecință.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/yak-shi-peretvoryvsya-na-mashynu-dezinformatsiyi/?utm_source=responsabil) și a fost tradus în limba română.
