---
title: "UE dezvoltă Age Verification Blueprint — un sistem real de verificare a vârstei pe internet"
date: 2026-04-09
draft: false
description: "UE pregătește Age Verification Blueprint, un portofel digital pentru verificarea vârstei online fără a dezvălui identitatea, înlocuind simplele butoane de confirmare a vârstei."
categories: ["securitate"]
cover:
  image: "images/cybercalm/ue-dezvolta-age-verification-blueprint-sistem-real-de-verificare-a-varstei-pe-internet.webp"
  alt: ""
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Uniunea Europeană se pregătește să înlocuiască butonul simbolic „am deja 18 ani” cu un sistem tehnic real de verificare a vârstei. În urma investigațiilor oficiale împotriva marilor platforme pornografice și Snapchat, Comisia Europeană promovează conceptul așa-numitului Age Verification Blueprint — un portofel digital pentru verificarea vârstei fără dezvăluirea datelor cu caracter personal.

## Ce a precedat schimbările

În mai 2025, Comisia Europeană a deschis proceduri oficiale împotriva Pornhub, Stripchat, XNXX și XVideos sub suspiciunea de încălcare a Actului privind serviciile digitale (Digital Services Act, DSA). Această lege, intrată în vigoare în 2024, obligă platformele mari să respecte transparența, să elimine rapid conținutul ilegal și să gestioneze riscurile sistemice — în special, să protejeze minorii.

În martie 2026, investigația a ajuns la concluzii preliminare: toate cele patru site-uri permit minorilor să acceseze serviciile lor printr-o simplă confirmare printr-un singur clic. Comisia Europeană a considerat acest mecanism complet inacceptabil din punctul de vedere al cerințelor legale.

În paralel, Snapchat a intrat în vizorul Comisiei. Conform rezultatelor unei investigații separate, platforma ar fi încălcat probabil DSA, expunând minorii riscului de grooming și recrutare pentru scopuri infracționale, precum și conținutului legat de vânzarea de droguri, țigări electronice și alcool.

DSA nu obligă direct platformele să implementeze verificarea vârstei, totuși, pentru așa-numitele platforme online foarte mari (Very Large Online Platforms, VLOP) — cele cu peste 45 de milioane de utilizatori activi lunar în UE — Comisia se așteaptă la pași concreți pentru reducerea riscurilor sistemice legate de protecția copiilor. Amenda pentru nerespectare poate ajunge la 18 milioane de euro sau 10% din cifra de afaceri globală anuală a companiei.

## Cum va funcționa Age Verification Blueprint

Într-o conferință de presă la care au participat oficialii Comisiei Europene, Prabhat Agarwal și Renate Nikolay, a fost explicat conceptul tehnic al noului sistem. Scopul acestuia este de a confirma că utilizatorul a atins o anumită vârstă fără a transmite platformei numele, data nașterii sau orice alte date personale.

Age Verification Blueprint este o aplicație mobilă care funcționează ca un portofel digital. Utilizatorul descarcă aplicația, își confirmă vârsta o singură dată folosind cartea electronică de identitate, pașaportul, o aplicație bancară sau un alt sistem național de identificare — iar după aceea poate dovedi că a împlinit 18 ani pe orice site compatibil, fără a prezenta documentele de fiecare dată de la zero.

La baza sistemului stă principiul *selective disclosure* — dezvăluirea selectivă a datelor. Aplicația nu comunică site-ului data nașterii utilizatorului. Aceasta răspunde doar la întrebarea „A atins această persoană vârsta de 18 ani?” cu un „da” sau „nu” verificat criptografic. Datele de identificare sunt transmise sub formă de token-uri de unică folosință, ceea ce, teoretic, face imposibilă urmărirea activității între diferite sesiuni pe același site.

## Legătura cu identitățile digitale paneuropene

Age Verification Blueprint a fost dezvoltat ca un pas intermediar către portofelele europene pentru identitate digitală (EU Digital Identity Wallets, EUDI Wallets), pe care unele țări UE trebuie să le implementeze până la sfârșitul anului 2026. Aceste portofele vor permite cetățenilor să stocheze într-o singură aplicație nu doar dovada vârstei, ci și cartea de identitate, documentele de studii, permisul de conducere și alte atribute personale.

Cinci state membre UE participă deja anul acesta la testarea pilot a sistemului, însă progresul este inegal. La conferința de presă s-a menționat că Franța și Danemarca au avansat considerabil, în timp ce Grecia, Spania și Italia au rămas în urmă. Din acest motiv, unii experți sunt sceptici în ceea ce privește realismul implementării portofelului digital în termenele stabilite.

## Alternative și experiența americană

Pe piața europeană a verificării vârstei sunt deja prezenți câțiva jucători. De exemplu, Yoti — serviciu pe care TikTok îl folosește în Europa alături de alte metode de verificare, cum ar fi cardurile de credit și documentele. Un alt exemplu este Persona, utilizat de Roblox, Discord și Reddit.

Modelul Persona demonstrează clar riscurile pe care Comisia Europeană dorește să le evite. Serviciul colectează amprente, folosește recunoașterea facială, compară înfățișarea cu baze de date și păstrează aceste date timp de până la trei ani. În februarie 2026, s-a aflat că Persona a deschis public accesul la mii de fișiere pe internet. Compania a declarat că a fost vorba despre un mediu de testare izolat și că datele reale ale utilizatorilor nu au fost afectate, precum și că nu transmite date structurilor guvernamentale din SUA.

Experiența americană arată, în general, riscurile sistemelor de verificare bazate pe colectarea masivă a datelor de identificare. Comisia Europeană promovează un alt concept: nu „dovedește cine ești pentru ca eu să îți verific vârsta”, ci „pur și simplu dovedește-ți vârsta fără a dezvălui nimic în plus”. Arhitectura sistemului este deschisă (open source), ceea ce permite atât statelor membre, cât și jucătorilor de pe piață să dezvolte versiuni naționale sau derivate. Printre furnizorii europeni promițători menționați la conferința de presă se numără Scytales și T-Systems.

Comisia a descris, de asemenea, o arhitectură „triunghiulară” a sistemului: o terță parte confirmă că utilizatorul corespunde caracteristicii necesare — în special, că a atins vârsta necesară — fără a transmite site-ului niciun document sau date personale. Pentru a simplifica înțelegerea conceptului, Comisia a oferit analogia cu certificatele COVID.

## O vulnerabilitate evidentă

În ciuda perspectivelor tehnice, rămâne un decalaj semnificativ între promisiunile sistemului și realitatea socială. După cum s-a menționat la conferința de presă, Age Verification Blueprint vizează în primul rând ca site-ul să afle cât mai puține despre utilizator — dar nu rezolvă în niciun fel cea mai simplă metodă de eludare: un minor poate folosi telefonul, datele de cont sau documentele unui adult. Astfel, sistemul ar putea reduce volumul datelor personale aflate în circulație, dar nu va elimina automat riscul eludării efective a verificării vârstei.

Cu toate acestea, Age Verification Blueprint pare în prezent cea mai promițătoare soluție. Comisia Europeană a precizat că aceasta nu este singura variantă posibilă: ușile sunt deschise pentru alternative, cu condiția ca acestea să fie „la fel de eficiente”. Pornhub participă deja la faza pilot, iar alți operatori au fost, de asemenea, invitați să participe.

Astfel, Uniunea Europeană ar putea deveni primul mare „laborator” în care verificarea vârstei se transformă dintr-o formalitate într-o infrastructură reală — cu toate avantajele și riscurile pe care le implică acest lucru.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/perevirka-viku-age-verification-blueprint/?utm_source=responsabil) și a fost tradus în limba română.
