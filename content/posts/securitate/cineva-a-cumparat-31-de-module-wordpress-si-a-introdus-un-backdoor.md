---
title: "Cineva a cumpărat 31 de module WordPress și a introdus un backdoor în fiecare dintre ele"
date: 2026-04-16
draft: false
description: "Un atacator necunoscut a achiziționat 31 de module WordPress populare și a introdus un backdoor activat după 8 luni. WordPress.org a eliminat toate modulele afectate."
categories: ["securitate"]
cover:
  image: "images/cybercalm/cineva-a-cumparat-31-de-module-wordpress-si-a-introdus-un-backdoor.webp"
  alt: ""
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Un atacator necunoscut a achiziționat pe piața Flippa un portofoliu de peste 30 de module WordPress gratuite, cu o reputație de mulți ani — și a adăugat în fiecare dintre ele un backdoor ascuns. Codul malițios a existat discret pe site-uri timp de opt luni înainte de a fi activat în aprilie 2026. WordPress.org a închis toate cele 31 de module într-o singură zi.

## **Cumpărarea reputației: cum a început totul**

Portofoliul de module numit Essential Plugin (fostul WP Online Support) a fost construit de o echipă de dezvoltatori indieni începând cu anul 2015. Timp de peste zece ani, aceștia au creat peste 30 de plugin-uri gratuite cu versiuni premium: slidere, galerii, cronometre, ferestre pop-up, testimoniale etc.

La sfârșitul anului 2024, veniturile afacerii au scăzut cu 35–45%, iar unul dintre fondatori a scos întregul portofoliu la vânzare prin platforma Flippa. Cumpărătorul, cunoscut doar sub numele de „Kris”, cu experiență în SEO, criptomonede și marketing pentru jocuri de noroc, a achiziționat afacerea pentru o sumă de șase cifre. Flippa a publicat chiar și un studiu de caz despre această tranzacție în iulie 2025.

Primul commit SVN al noului proprietar s-a dovedit a fi un backdoor. Fondatorul companiei de găzduire Anchor Hosting, Austin Ginder, [a publicat](https://anchor.host/someone-bought-30-wordpress-plugins-and-planted-a-backdoor-in-all-of-them/) pe blogul său o descriere detaliată a atacului asupra lanțului de aprovizionare.

## **Backdoor: opt luni de așteptare**

Pe 8 august 2025, noul proprietar a lansat versiunea 2.6.7 a modului Countdown Timer Ultimate. În jurnalul de modificări era menționată doar „verificarea compatibilității cu WordPress 6.8.2”. În realitate, actualizarea adăuga un modul ascuns care îi permitea atacatorului să controleze site-ul de la distanță.

Codul malițios nu a făcut nimic timp de opt luni — până pe 5–6 aprilie 2026, când atacul a fost activat. Modulul a contactat un server extern și a descărcat un fișier cu un nume intenționat asemănător cu un fișier standard WordPress. Ulterior, un bloc masiv de cod ascuns a fost injectat în fișierul de configurare al site-ului, `wp-config.php`.

Software-ul malițios afișa link-uri de spam și pagini false doar roboților motoarelor de căutare — proprietarii site-urilor nu vedeau nimic. Pentru a îngreuna blocarea, atacatorii au folosit adresa serverului de control codificată într-un smart contract Ethereum: blocarea tradițională a domeniului nu ar fi funcționat, deoarece noua adresă poate fi actualizată direct în blockchain.

## **WordPress.org a închis toate modulele într-o singură zi**

Pe 7 aprilie 2026, echipa WordPress.org Plugins Team a închis definitiv toate cele 31 de module ale autorului essentialplugin. Pe 8 aprilie, platforma a forțat actualizarea modulelor pe toate site-urile la versiunea 2.6.9.1, care a neutralizat mecanismul de comunicare cu serverul atacatorului. Cu toate acestea, actualizarea forțată nu a curățat fișierul `wp-config.php` — dacă site-ul primise deja codul malițios, acesta continua să funcționeze.

## **Lista modulelor afectate**

Verificați site-ul pentru prezența oricăruia dintre modulele de mai jos și ștergeți-le imediat:

* Accordion and Accordion Slider
* Album and Image Gallery Plus Lightbox
* Audio Player with Playlist Ultimate
* Blog Designer for Post and Widget
* Countdown Timer Ultimate
* Featured Post Creative
* Footer Mega Grid Columns
* Hero Banner Ultimate
* HTML5 VideoGallery Plus Player
* Meta Slider and Carousel with Lightbox
* Popup Anything on Click
* Portfolio and Projects
* Post Category Image with Grid and Slider
* Post Grid and Filter Ultimate
* Preloader for Website
* Product Categories Designs for WooCommerce
* Responsive WP FAQ with Category (sp-faq)
* SlidersPack — All in One Image Sliders
* SP News And Widget
* Styles for WP PageNavi — Addon
* Ticker Ultimate
* Timeline and History Slider
* Woo Product Slider and Carousel with Category
* WP Blog and Widgets
* WP Featured Content and Slider
* WP Logo Showcase Responsive Slider and Carousel
* WP Responsive Recent Post Slider
* WP Slick Slider and Image Carousel
* WP Team Showcase and Slider
* WP Testimonial with Widget
* WP Trending Post Slider and Widget

## **Ce trebuie să faceți: pași de urmat**

1. **Verificați lista modulelor instalate.** În panoul de control WordPress, mergeți la secțiunea „Module” și comparați cu lista de mai sus.
2. **Dezactivați și ștergeți modulele afectate.** Nu doar le dezactivați — ștergeți-le complet. Căutați alternative de la autori verificați.
3. **Verificați fișierul wp-config.php.** Deschideți fișierul prin managerul de fișiere al găzduirii sau prin FTP. Dimensiunea normală este de aproximativ 3–4 KB. Dacă fișierul este semnificativ mai mare (peste 6 KB) sau dacă vedeți cod suspect la sfârșitul liniei `require_once ABSPATH . 'wp-settings.php'`, site-ul este compromis.
4. **Dacă wp-config.php este infectat — contactați un specialist.** Simpla ștergere a modului nu va ajuta: este necesară o curățare completă a site-ului, verificarea tuturor fișierelor și, eventual, restaurarea dintr-o copie de rezervă creată înainte de 5 aprilie 2026.
5. **Verificați copiile de rezervă.** Comparați dimensiunea `wp-config.php` în copiile de rezervă din diferite date. Dacă acestea sunt stocate pe hosting, asistența tehnică vă poate ajuta să stabiliți momentul exact al infecției.
6. **Schimbați parolele.** După curățarea site-ului, schimbați parolele de administrator WordPress, ale bazei de date și ale contului de găzduire.
7. **Instalați un modul de securitate.** Plugin-uri precum Wordfence sau iThemes Security vă vor ajuta să detectați modificările suspecte ale fișierelor în viitor.
8. **Urmăriți notificările WordPress.org.** Când platforma închide un modul din motive de securitate, în panoul de control WordPress apare o avertizare corespunzătoare. Nu ignorați niciodată aceste mesaje.

## **Problemă sistemică: WordPress nu verifică noii proprietari ai modulelor**

Acesta nu este primul caz de acest gen. Cu o săptămână înainte, un atac similar a fost descoperit în modulul Widget Logic. În 2017, cumpărătorul modului Display Widget (200.000 de instalări active) a introdus, de asemenea, cod de spam după achiziție.

WordPress.org nu are niciun mecanism pentru verificarea schimbării proprietarului unui modul. Nici notificări pentru utilizatori, nici verificări suplimentare ale codului la apariția unui nou commit. Echipa de securitate a platformei a reacționat rapid după descoperirea atacului — dar între introducerea backdoor-ului și detectarea acestuia au trecut opt luni.

Acest incident ilustrează un risc major al lanțului de aprovizionare software: chiar și un instrument de încredere, folosit de ani de zile, poate deveni o amenințare după schimbarea proprietarului. Verificați cine dezvoltă modulele pe care le folosiți și urmăriți schimbările de autor.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/htos-kupyv-31-wordpress-plagin-i-vbuduvav-bekdor/?utm_source=responsabil) și a fost tradus în limba română.
