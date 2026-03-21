---
title: "O vulnerabilitate critică în Chrome permite extensiilor malițioase să spioneze utilizatorii prin intermediul Gemini"
date: 2026-03-03
draft: false
description: "Cercetătorii au descoperit o vulnerabilitate în Chrome care, prin Gemini, permite extensiilor malițioase să fure date și să acceseze camera/microfonul. Actualizați browserul imediat."
categories: ["securitate"]
cover:
  image: "images/cybercalm/vulnerabilitate-critica-chrome-extensii-malitioase-gemini.webp"
  alt: ""
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Cercetătorii în domeniul securității au descoperit o vulnerabilitate cu grad ridicat de risc în funcția Gemini a browserului Google Chrome. Aceasta permite atacatorilor să utilizeze extensii malițioase pentru a fura date, a accesa camera web și microfonul. Actualizarea este deja disponibilă.

## **Esența vulnerabilității**

Vulnerabilitatea, căreia i-a fost atribuit identificatorul [CVE-2026-0628](https://nvd.nist.gov/vuln/detail/CVE-2026-0628) și statutul de „pericol ridicat”, a fost descoperită de Gal Weizman, cercetător principal de securitate în cadrul echipei Unit 42 a companiei Palo Alto Networks. Problema este clasificată drept „aplicare insuficientă a politicilor în tag-ul WebView al browserului Google Chrome” și afectează toate versiunile Chrome anterioare versiunii 143.0.7499.192.

Tehnic, vulnerabilitatea constă în faptul că o extensie cu un set de permisiuni de bază — prin API-ul declarativeNetRequests — ar putea obține privilegii care în condiții normale nu îi sunt disponibile. Un atacator, convingând utilizatorul să instaleze o extensie malițioasă, ar putea injecta cod JavaScript într-un nou component al panoului Gemini.

## **Posibile consecințe ale atacului**

Conform evaluării cercetătorilor, vulnerabilitatea poate fi utilizată ca parte a unui lanț mai larg de atacuri asupra utilizatorilor Chrome. Dacă atacatorul reușește să convingă victima să descarce o extensie aparent sigură, aceasta este capabilă să preia controlul asupra asistentului AI Gemini. Ulterior, Gemini poate acționa fără știrea sau acordul utilizatorului: să ofere cibercriminalilor acces la camera web și microfon, să facă capturi de ecran, precum și să citească fișiere și directoare locale.

Panoul Gemini poate fi, de asemenea, interceptat pentru atacuri de phishing. „Deoarece aplicația Gemini efectuează acțiuni în scopuri legitime, capturarea panoului său oferă acces privilegiat la resursele sistemului, pe care o extensie în regim normal nu l-ar putea obține”, au menționat cercetătorii.

## **Cum să te protejezi**

După ce Palo Alto Networks a notificat Google în privat despre vulnerabilitate în luna octombrie a anului trecut, echipa de securitate Chrome a dezvoltat o soluție. Patch-ul a fost inclus în versiunile canalelor stabile Chrome 143.0.7499.192/.193 pentru Windows și macOS și versiunea 143.0.7499.192 pentru Linux.

Sfatul este simplu: de îndată ce în colțul din dreapta sus al browserului apare o notificare despre o actualizare disponibilă — acceptați-o imediat. Acest lucru nu numai că va elimina vulnerabilitatea descrisă, dar va proteja și împotriva altor amenințări cunoscute, inclusiv erorile de depășire a limitelor buffer-ului, corectate în actualizările ulterioare.

## **Browserul agent: o nouă zonă de risc**

Browserele agent — software care combină un browser tradițional cu inteligența artificială capabilă să execute sarcini în mod autonom — devin un model tot mai răspândit de navigare web. Acestea răspund la solicitări, găsesc informații, completează formulare și ajută la gestionarea proceselor de lucru. În același timp, transferul controlului asupra conturilor online și datelor personale către instrumentele AI creează provocări fundamental noi pentru securitatea cibernetică.

Una dintre amenințările cheie o reprezintă atacurile de tip prompt injection: instrucțiunile malițioase ascunse în conținutul site-urilor pot intercepta agenții AI și îi pot forța să transmită date confidențiale sau să execute acțiuni nedorite. Un studiu recent al Institutului Tehnologic din Massachusetts (MIT) a înregistrat lacune serioase în testarea securității sistemelor AI de tip agent în procesul dezvoltării lor accelerate, ceea ce necesită o atitudine prudentă față de astfel de tehnologii.

„Inovația nu poate avea loc în detrimentul securității”, a subliniat Anupam Upadhyaya, vicepreședinte senior pentru managementul produselor Prisma SASE la Palo Alto Networks. „Dacă organizațiile decid să implementeze browsere agent, trebuie să le considere ca pe o infrastructură cu nivel ridicat de risc — cu vizibilitate în timp real, control al aplicării politicilor și măsuri de protecție consolidate de la începutul implementării. Orice altă abordare este o invitație la compromitere”.

Amploarea totală a riscurilor purtate de sistemele AI agent nu este încă dezvăluită — la fel ca și adevăratul lor potențial. Sarcina constă în găsirea unui echilibru între utilitate și securitate, iar acest lucru este valabil atât pentru utilizatorii obișnuiți, cât și pentru sectorul corporativ.

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/krytychna-vrazlyvist-chrome-cve-2026-0628/) și a fost tradus în limba română.