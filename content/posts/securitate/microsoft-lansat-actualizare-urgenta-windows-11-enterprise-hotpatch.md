---
title: "Microsoft a lansat o actualizare de urgență pentru Windows 11 Enterprise cu hotpatch"
date: 2026-03-15
draft: false
description: "Microsoft a lansat actualizarea KB5084597 pentru Windows 11 Enterprise, rezolvând vulnerabilități critice în serviciul RRAS prin tehnologia hotpatch, fără a necesita repornirea sistemului."
categories: ["securitate"]
cover:
  image: "images/cybercalm/microsoft-lansat-actualizare-urgenta-windows-11-enterprise-hotpatch.png"
  alt: ""
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Microsoft a lansat un hotpatch neplanificat pentru Windows 11 Enterprise pentru a remedia vulnerabilități critice în instrumentul de gestionare RRAS (Routing and Remote Access Service), care pot duce la executarea de cod la distanță.

## Ce s-a întâmplat
Actualizarea KB5084597 a fost lansată pe 10 martie — nu în obișnuita „marți a patch-urilor” (Patch Tuesday), ci separat. Aceasta corectează trei vulnerabilități (CVE-2026-25172, CVE-2026-25173 și CVE-2026-26111), care permit unui atacator să execute cod pe dispozitiv dacă utilizatorul se conectează la un server malițios prin intermediul instrumentului RRAS.
Conform Microsoft, vulnerabilitățile vizează doar un număr limitat de scenarii: dispozitivele corporative cu Windows 11 care primesc actualizări de tip hotpatch și sunt utilizate pentru gestionarea de la distanță a serverelor.
„Un atacator autentificat în domeniu poate exploata această vulnerabilitate forțând un utilizator de domeniu să trimită o cerere către un server malițios prin intermediul snap-in-ului RRAS”, se precizează în descrierea celor trei vulnerabilități.

## Ce este hotpatch și de ce este important
De obicei, instalarea actualizărilor de securitate Windows necesită repornirea dispozitivului. Însă unele sisteme corporative funcționează non-stop și nu pot fi repornite ușor — de exemplu, serverele de infrastructură critică sau sistemele de control al producției.
Hotpatch este o tehnologie Microsoft care permite instalarea patch-urilor „din mers”: procesele care rulează în memorie sunt actualizate, iar fișierele de pe disc sunt modificate astfel încât, după următoarea repornire, corecțiile să rămână active. Repornirea nu este necesară.

## Cui îi este adresată această actualizare
Actualizarea hotpatch este disponibilă doar pentru:

Windows 11 versiunile 24H2 și 25H2
Windows 11 Enterprise LTSC 2024
Dispozitivele înregistrate în programul hotpatch și gestionate prin Windows Autopatch

Pentru aceste dispozitive, actualizarea se instalează automat, fără repornire. Restul utilizatorilor Windows 11 au primit corecțiile pentru aceste vulnerabilități în actualizarea standard din 10 martie (Patch Tuesday) — dar cu necesitatea repornirii sistemului.

## De ce Microsoft a lansat actualizarea de două ori
Microsoft menționează că a lansat anterior un hotfix pentru aceste vulnerabilități, dar a relansat patch-ul „pentru a asigura acoperirea completă a tuturor scenariilor afectate”. Aceasta înseamnă că prima versiune de hotpatch s-ar fi putut să nu protejeze anumite configurații de sistem.

## Ce trebuie să facă utilizatorii
Dacă utilizați o versiune obișnuită de Windows 11 (nu Enterprise) sau nu lucrați cu instrumente de gestionare la distanță a serverelor — aceste vulnerabilități nu vă vizează. Este suficient să instalați actualizările standard Windows prin Windows Update.
Dacă organizația dumneavoastră utilizează Windows 11 Enterprise cu hotpatch — verificați dacă actualizarea KB5084597 s-a instalat automat. Administratorii ar trebui să se asigure că toate dispozitivele care gestionează servere prin RRAS au primit patch-ul.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/microsoft-windows-11-enterprise-hotpatch-rras/) și a fost tradus în limba română.