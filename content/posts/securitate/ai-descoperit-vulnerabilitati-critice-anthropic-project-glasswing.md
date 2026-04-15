---
title: "AI a descoperit mii de vulnerabilități critice în principalele sisteme de operare și browsere — Anthropic prezintă Project Glasswing"
date: 2026-04-09
draft: false
description: "Anthropic lansează Project Glasswing, o inițiativă de securitate cibernetică ce utilizează AI-ul Claude Mythos Preview pentru a identifica mii de vulnerabilități critice în software-ul global."
categories: ["securitate"]
cover:
  image: "images/cybercalm/ai-descoperit-vulnerabilitati-critice-anthropic-project-glasswing.webp"
  alt: ""
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Anthropic a anunțat Project Glasswing — o inițiativă masivă de securitate cibernetică intersectorială, la care s-au alăturat Amazon Web Services, Apple, Cisco, CrowdStrike, Google, JPMorganChase, Microsoft, NVIDIA, Palo Alto Networks, Broadcom și Linux Foundation. La baza inițiativei se află cel mai nou model, Claude Mythos Preview, care a găsit deja mii de vulnerabilități critice zero-day în toate sistemele de operare și browserele majore, unele dintre ele existând neobservate de decenii.

**Ce este Project Glasswing**
[Project Glasswing](https://www.anthropic.com/glasswing) este o inițiativă de apărare comună, al cărei scop este de a pune cele mai puternice capacități AI din domeniul securității cibernetice în serviciul protecției, nu al atacului. Catalizatorul a fost demonstrația capacităților Claude Mythos Preview — noul model închis al Anthropic care, conform companiei, depășește majoritatea experților umani în detectarea și exploatarea vulnerabilităților software.

Participanții la program vor avea acces la Mythos Preview pentru a căuta vulnerabilități în sistemele lor cheie — cele care formează o parte semnificativă a suprafeței comune de amenințări cibernetice la nivel mondial. Se așteaptă ca activitatea să se concentreze pe detectarea locală a vulnerabilităților, testarea fișierelor binare prin metoda „black box”, protecția endpoint-urilor și testarea de penetrare a sistemelor.

**Ce a descoperit deja Claude Mythos Preview**
În doar câteva săptămâni de utilizare, modelul a identificat mii de vulnerabilități zero-day — adică cele care erau anterior necunoscute dezvoltatorilor software-ului respectiv. Aceste vulnerabilități acoperă toate sistemele de operare majore și toate browserele principale, precum și o gamă largă de alte software-uri critice. Este remarcabil faptul că modelul a făcut majoritatea descoperirilor în mod complet autonom, fără intervenție umană.

Printre exemplele specifice dezvăluite după remediere se numără:


- **Vulnerabilitate de 27 de ani în OpenBSD** — sistem de operare considerat unul dintre cele mai sigure din lume și utilizat pentru firewall-uri și alte infrastructuri critice. Vulnerabilitatea permitea unui atacator să oprească de la distanță orice dispozitiv doar prin conectarea la acesta;

- **Vulnerabilitate de 16 ani în FFmpeg** — o bibliotecă utilizată pe scară largă pentru codificarea și decodificarea video. Problema se afla într-o linie de cod pe care instrumentele automate de testare o verificaseră de cinci milioane de ori fără a o detecta;

- **Lanț de vulnerabilități în kernel-ul Linux** — software-ul care asigură funcționarea majorității serverelor din lume. Combinând mai multe vulnerabilități, modelul a reușit să demonstreze o cale de la drepturile de utilizator obișnuit la controlul total asupra mașinii.

Toate cele trei vulnerabilități au fost deja remediate. Pentru un număr semnificativ de alte descoperiri, Anthropic a publicat un hash criptografic al detaliilor și va dezvălui specificul după lansarea patch-urilor de corecție.

**Comparație cu modelele anterioare**
Pe benchmark-ul CyberGym, care evaluează reproducerea vulnerabilităților, Mythos Preview a obținut 83,1% față de 66,6% pentru Claude Opus 4.6. Un avans similar se observă și în sarcinile generale de dezvoltare software: pe SWE-bench Verified modelul a atins 77,8% față de 53,4%, iar pe Terminal-Bench 2.0 — 93,9% față de 80,8% pentru Opus 4.6.

**De ce este acest lucru important pentru apărarea cibernetică**
După cum explică cei de la Anthropic, aceeași capacitate care face un model AI periculos în mâinile atacatorilor îl face neprețuit pentru apărători: anterior, căutarea și eliminarea vulnerabilităților necesitau o expertiză rară și un consum semnificativ de timp. Acum, același proces poate fi scalat.

O preocupare deosebită este faptul că capacități similare ar putea apărea în curând la atacatori. Dacă astăzi găsirea și exploatarea unei vulnerabilități critice este posibilă doar pentru cei mai calificați specialiști, pe măsură ce modelele AI puternice se răspândesc, această barieră va scădea rapid. Ca răspuns, Project Glasswing urmărește să ofere apărătorilor un avantaj înainte ca această schimbare să aibă loc.

La un nivel geopolitic mai larg, Anthropic atrage atenția asupra amenințărilor din partea actorilor statali — în special cei legați de Rusia, China, Iran și Coreea de Nord — și subliniază că protejarea infrastructurii critice este o prioritate de securitate națională pentru țările democratice.

**Angajamente financiare și acces**
Anthropic alocă până la 100 de milioane de dolari sub formă de credite pentru utilizarea Mythos Preview pentru participanții la program. În plus, compania transferă 2,5 milioane de dolari organizațiilor Alpha-Omega și OpenSSF prin intermediul Linux Foundation și 1,5 milioane de dolari către Apache Software Foundation pentru a sprijini menținătorii de software open source.

Accesul la model a fost deja acordat pentru peste 40 de organizații care dezvoltă sau susțin infrastructură software critică. După finalizarea preview-ului de cercetare, Mythos Preview va fi disponibil participanților la prețul de 25 USD per milion de tokeni de intrare și 125 USD per milion de tokeni de ieșire — prin Claude API, Amazon Bedrock, Google Cloud Vertex AI și Microsoft Foundry.

**Ce urmează**
Anthropic nu intenționează să ofere Claude Mythos Preview pentru acces general. Compania dezvoltă mijloace de protecție menite să detecteze și să blocheze cele mai periculoase rezultate ale modelului și intenționează să le implementeze odată cu viitoarea lansare Claude Opus. În decurs de 90 de zile, Anthropic promite să raporteze public rezultatele: numărul de vulnerabilități remediate, lecțiile învățate și recomandări practice privind modul în care ar trebui să se schimbe abordările de securitate în era AI.

Pe termen mai lung, compania contează pe formarea unui organism industrial independent — cu reprezentanți ai sectoarelor privat și public — care să poată prelua responsabilitatea pentru proiecte cibernetice la scară largă, similare cu Project Glasswing.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/anthropic-ogoloshuye-project-glasswing/?utm_source=responsabil) și a fost tradus în limba română.
