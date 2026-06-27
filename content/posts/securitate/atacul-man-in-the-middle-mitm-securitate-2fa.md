---
title: "Atacul „Man-in-the-Middle” (MITM): de ce 2FA nu mai este suficientă și ce oferă protecție reală"
date: 2026-06-24
draft: false
description: "Află cum funcționează atacurile MITM moderne, de ce autentificarea în doi pași poate fi ocolită prin tehnici AiTM și cum passkeys oferă cea mai bună protecție."
categories: ["securitate"]
tags: ["securitate cibernetică", "atac mitm", "autentificare 2fa", "passkeys", "protecție date", "phishing"]
cover:
  image: "images/cybercalm/atacul-man-in-the-middle-mitm-securitate-2fa.webp"
  alt: "Diagramă explicativă a unui atac Man-in-the-Middle în care un atacator interceptează traficul între utilizator și server."
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Imaginează-ți o dimineață obișnuită: deschizi e-mailul de serviciu, introduci parola, confirmi accesul pe telefon — și te apuci liniștit de treabă. Dar în acea secundă, altcineva este deja în contul tău. Ai făcut totul „corect”, ai trecut chiar și de autentificarea în doi pași — și tocmai de aceea atacul a funcționat. Aceasta este fața modernă a amenințării numite clasic „omul de la mijloc” (man-in-the-middle, MITM). Să analizăm cum funcționează astăzi și ce ajută cu adevărat la protecție.

## **Ce este un atac „Man-in-the-Middle”**

Un atac „man-in-the-middle” are loc atunci când un atacator se [interpune invizibil între tine și site-ul sau aplicația](https://attack.mitre.org/techniques/T1557/) cu care comunici. Acesta fie interceptează schimbul de date, fie simulează una dintre părți, astfel încât să fii convins că totul decurge normal. Scopul este de a obține informații de valoare: date de autentificare, date bancare sau acces la conturi corporative.

O analogie simplă: este ca un poștaș care deschide scrisoarea de la bancă, modifică datele, sigilează plicul cu grijă și îl pune în cutia poștală. La exterior, nimic nu pare schimbat.

Un detaliu important: atacatorul nu trebuie să fie la computerul tău sau în aceeași țară. Uneori este suficient să fie în aceeași rețea — sau să te păcălească să te conectezi la a lui. Experții în securitate folosesc acum mai des termenul „adversar la mijloc” (adversary-in-the-middle, AiTM), deoarece atacul poate fi realizat nu doar de o persoană, ci de un instrument automatizat.

## **Cele două fețe ale MITM**

În ultimii ani, această amenințare a dezvoltat două scenarii foarte diferite. Primul este cel clasic, la nivel de rețea. Al doilea este mai nou și este cel care provoacă în prezent cele mai mari daune.

### **Atacul clasic: Wi-Fi fals și spoofing**

Cel mai cunoscut scenariu este Wi-Fi-ul public în locuri aglomerate. Oamenii văd „Wi-Fi gratuit” și se conectează fără să se gândească cine este în spate. Crearea unui punct de acces fals este mai simplă decât pare: atacatorul dă rețelei un nume similar cu cel al locației, o lasă fără parolă și, imediat ce te-ai conectat, are acces la traficul tău. [Aeroporturile, cafenelele și bibliotecile](https://cybercalm.org/yak-bezpechno-korystuvatysya-publichnym-wi-fi-porady-dlya-zahystu-vashyh-danyh/) sunt locuri tipice pentru astfel de puncte de acces.

Metode mai active de intervenție în rețea:

*   **ARP Spoofing** — atacatorul își asociază adresa cu cea a unui dispozitiv legitim din rețeaua locală, iar datele pe care le trimiți ajung la el.
*   **DNS Spoofing** ([otrăvirea cache-ului](https://cybercalm.org/dns-cache-poisoning/)) — cererea pentru adresa unui site este deturnată, iar tu ajungi pe o copie controlată de atacator.
*   **IP Spoofing** — antetele pachetelor de rețea sunt modificate pentru a te redirecționa către o resursă străină.

Vestea bună: acest tip de atacuri a slăbit considerabil. În trecut, o parte din web funcționa prin HTTP nesecurizat, astfel încât traficul putea fi citit ușor (SSL stripping). Astăzi, marea majoritate a site-urilor folosesc HTTPS, browserele avertizează despre conexiunile nesigure, iar tehnologii precum HSTS previn retrogradarea site-ului la HTTP.

### **Atacul modern: Proxy-ul care îți fură sesiunea (AiTM)**

Aici s-a mutat pericolul. Astăzi, cel mai răspândit scenariu MITM nu este „cineva în Wi-Fi-ul tău”, ci phishing-ul prin reverse proxy. Funcționează astfel: primești un e-mail convingător cu un link către o „pagină de autentificare”. Pagina arată real — deoarece atacatorul îți transmite în timp real site-ul oficial prin serverul său. Introduci datele, treci de 2FA — totul funcționează. Dar în acel moment, proxy-ul interceptează nu doar parola, ci și [cookie-ul de sesiune — „permisul” digital pe care site-ul îl emite după autentificarea reușită](https://www.proofpoint.com/us/blog/email-and-cloud-threats/aitm-phishing-attacks-evolving-threat-microsoft-365).

Având acest cookie, atacatorul îl încarcă în propriul browser și se trezește în contul tău deja autentificat, fără a mai fi nevoie de parolă sau cod. Kiturile gata făcute pentru astfel de atacuri (precum Evilginx sau Tycoon 2FA) au făcut acest scenariu unul de masă. Principalele ținte sunt e-mailurile, conturile Microsoft 365, Google Workspace și băncile.

## **De ce 2FA nu mai este suficientă**

Ani de zile ni s-a spus: activează autentificarea în doi pași și parola furată va fi inutilă. Pentru phishing-ul obișnuit, acest lucru este încă adevărat. Dar AiTM nu încearcă să „spargă” al doilea factor — așteaptă ca tu să îl treci cu succes și fură rezultatul: sesiunea gata creată. Codurile SMS, codurile din aplicațiile de autentificare și chiar confirmările push nu te salvează aici, deoarece atacatorul le transmite site-ului real în locul tău.

Asta nu înseamnă că trebuie să dezactivezi 2FA — orice MFA este mai bună decât lipsa ei. Înseamnă însă că simplul fapt de a avea 2FA nu mai este egal cu „sunt în siguranță”.

## **Cum să te protejezi — de la cel mai important la cel de dorit**

1.  **Treci la passkeys (FIDO2) unde este posibil.** Aceasta este cea mai eficientă protecție împotriva AiTM. [Passkey-ul este legat criptografic de un domeniu specific](https://fidoalliance.org/passkeys/): o cheie creată pentru bank.com nu va funcționa pe un site fals, chiar dacă nu ai observat înlocuirea. Apple, Google și Microsoft susțin passkeys, iar autoritățile o consideră [„standardul de aur” al protecției](https://www.cisa.gov/sites/default/files/publications/fact-sheet-implementing-phishing-resistant-mfa-508c.pdf).
2.  **Ai încredere în avertismentele browserului.** Dacă browserul spune că o conexiune este nesigură sau certificatul este invalid, nu ignora avertismentul. Acesta este adesea singurul semnal vizibil al unui atac.
3.  **Atenție la Wi-Fi-ul public.** Evită rețelele deschise fără parolă și nu efectua operațiuni confidențiale (banking, e-mail de serviciu) din cafenele sau hoteluri. Dacă trebuie să le folosești, utilizează un VPN de încredere care criptează tot traficul.
4.  **Nu accesa paginile de autentificare prin link-uri din e-mailuri.** Deschide site-ul băncii sau al e-mailului manual, din bookmarks sau tastând adresa. Click-ul din e-mail este principala poartă pentru AiTM.
5.  **Închide sesiunile și nu rămâne logat permanent.** Deconectarea regulată reduce valoarea unui cookie furat.
6.  **Actualizează sistemul și browserul, verifică extensiile.** O extensie de browser malițioasă poate deveni „omul din browserul tău”.

## **Trei mituri de abandonat**

*   **„Am 2FA, deci sunt protejat.”** Împotriva AiTM nu este suficient; doar passkeys/FIDO2 oferă siguranță reală.
*   **„VPN-ul protejează de orice.”** VPN-ul criptează canalul, dar nu te oprește să introduci date pe o pagină falsă.
*   **„Este o amenințare doar pentru Wi-Fi public.”** Astăzi, majoritatea atacurilor MITM reușite încep cu un e-mail și o pagină de login falsă.

## **Întrebări frecvente**

**Mă protejează VPN-ul de un atac Man-in-the-Middle?**
Parțial. VPN-ul criptează traficul și protejează împotriva interceptării în rețele nesigure. Totuși, nu va opri phishing-ul AiTM dacă introduci singur datele pe o pagină falsă.

**Dacă am 2FA activat, pot fi victima unui atac MITM?**
Da. Atacurile AiTM moderne fură cookie-ul de sesiune după ce ai trecut de 2FA. Protecția reală este oferită de passkeys.

**Ce este un passkey?**
Este o cheie criptografică legată de un site specific și de dispozitivul tău. Nu poate fi furată prin phishing deoarece nu va funcționa pe un domeniu fals.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/shho-take-ataka-man-in-the-middle-ta-yak-sebe-zahystyty/?utm_source=responsabil) și a fost tradus în limba română.
