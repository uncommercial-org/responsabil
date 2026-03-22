---
title: "Agentul AI Meta a provocat o scurgere de date din cauza unui sfat inexact"
date: 2026-03-20
draft: false
description: "Un agent AI intern al Meta a cauzat un incident de securitate și acces neautorizat la datele companiei după ce a oferit unui inginer un sfat tehnic eronat."
categories: ["securitate"]
cover:
  image: "images/cybercalm/agentul-ai-meta-a-provocat-o-scurgere-de-date-din-cauza-unui-sfat-inexact.webp"
  alt: ""
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Săptămâna trecută, angajații Meta au avut acces neautorizat la datele interne ale companiei timp de aproape două ore din cauza unui agent AI care a oferit unui angajat un sfat tehnic inexact. Reprezentanta Meta, Tracy Clayton, a declarat pentru publicația [The Verge](https://www.theverge.com/ai-artificial-intelligence/897528/meta-rogue-ai-agent-security-incident) că, în timpul incidentului, „datele utilizatorilor nu au fost compromise”.

## Cum s-a produs eroarea

Un inginer Meta a utilizat un agent AI intern pentru a analiza o problemă tehnică pe care un alt angajat o postase pe forumul intern al companiei. Potrivit lui Clayton, acest agent este „similar prin natura sa cu OpenClaw într-un mediu de dezvoltare securizat”.

Problema a apărut atunci când agentul a publicat autonom — fără aprobare prealabilă — un răspuns public la întrebare după analiza acesteia. Răspunsul ar fi trebuit să fie afișat doar angajatului care l-a solicitat, nu tuturor angajaților.

## Consecințele incidentului

Unul dintre angajați a acționat conform sfatului agentului AI, care s-a dovedit a fi inexact. Acest lucru a dus la un incident de securitate de nivel SEV1 — al doilea cel mai grav nivel în clasificarea Meta. Drept urmare, angajații au primit temporar acces la date confidențiale pe care nu aveau dreptul să le vizualizeze. De atunci, problema a fost remediată.

Potrivit lui Clayton, agentul AI nu a efectuat nicio acțiune tehnică în afară de publicarea sfatului inexact — ceva ce ar fi putut face și o persoană obișnuită. Totuși, un om ar fi efectuat probabil verificări suplimentare înainte de a partaja informația.

> „Angajatul care a interacționat cu sistemul era pe deplin conștient de faptul că comunica cu un bot automatizat. Acest lucru a fost menționat în clauza de exonerare de răspundere din partea de jos a paginii, precum și în propriul răspuns al angajatului în discuție”, a comentat Clayton.

Ea a adăugat: „Agentul nu a efectuat nicio altă acțiune în afară de a oferi un răspuns la întrebare. Dacă inginerul care a acționat pe baza acestui sfat ar fi înțeles mai bine situația sau ar fi efectuat verificări suplimentare, acest lucru ar fi putut fi evitat”.

## Nu este primul caz

Luna trecută, un agent AI de pe platforma open-source OpenClaw a scăpat de sub control: o angajată i-a cerut să sorteze e-mailurile din inbox, iar acesta a început să șteargă e-mailurile fără permisiune.

Întreaga idee a unor astfel de agenți, precum OpenClaw, este că aceștia pot acționa independent. Dar, la fel ca orice alte modele AI, aceștia nu interpretează întotdeauna corect cererile și instrucțiunile și nu oferă întotdeauna răspunsuri precise. Angajații Meta s-au convins de acest lucru pentru a doua oară.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/meta-ai-agent-data-leak-incident/?utm_source=responsabil) și a fost tradus în limba română.
