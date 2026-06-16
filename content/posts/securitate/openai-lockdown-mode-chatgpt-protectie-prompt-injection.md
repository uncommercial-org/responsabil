---
title: "OpenAI a lansat Lockdown Mode în ChatGPT: un mod de protecție sporită împotriva atacurilor de tip prompt injection"
date: 2026-06-08
draft: false
description: "OpenAI extinde Lockdown Mode pentru toți utilizatorii ChatGPT, oferind protecție avansată împotriva furtului de date și a atacurilor de tip prompt injection prin restricționarea accesului web."
categories: ["securitate"]
tags: ["openai", "chatgpt", "securitate cibernetica", "prompt injection", "protectia datelor", "lockdown mode"]
cover:
  image: "images/cybercalm/openai-lockdown-mode-chatgpt-protectie-prompt-injection.webp"
  alt: "Interfața ChatGPT afișând activarea funcției Lockdown Mode pentru securitate sporită împotriva atacurilor cibernetice."
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

OpenAI a deschis accesul la Lockdown Mode — un mod suplimentar de securitate pentru ChatGPT, care restricționează strict interacțiunea aplicației cu serviciile externe și cu web-ul, pentru a reduce riscul de furt de date (exfiltrare) în urma atacurilor de tip prompt injection. Anterior, funcția era disponibilă doar pentru clienții enterprise, însă acum este extinsă la conturile personale Free, Go, Plus și Pro, precum și la conturile de business self-serve ale ChatGPT.


**Ce este Lockdown Mode**
Lockdown Mode este o setare opțională de securitate avansată care restricționează majoritatea instrumentelor și funcționalităților produselor OpenAI capabile să se conecteze la web sau la servicii externe. Protecția este realizată prin limitarea solicitărilor de rețea de ieșire, prin care un atacator ar putea extrage date confidențiale. Prețul acestei siguranțe este dezactivarea sau limitarea unor funcții utile.

Conform poziției OpenAI, acest mod nu este destinat tuturor. Este orientat către persoanele și organizațiile care lucrează cu date sensibile și au nevoie de o protecție mai strictă împotriva riscurilor de exfiltrare asociate cu prompt injection — de exemplu, pentru directori sau echipe de securitate din organizații proeminente.

Funcția a fost prezentată pentru prima dată pe 13 februarie 2026 pentru tarifele corporate — ChatGPT Enterprise, Edu, Healthcare și for Teachers. Conform actualizării anunțului OpenAI din 4 iunie 2026, modul a început să fie implementat și pentru conturile personale și business self-serve. Dacă Lockdown Mode nu a apărut încă în setări, este posibil să nu fie încă disponibil pentru contul respectiv.


**Cum funcționează un atac de tip prompt injection**
Prompt injection (injecția de prompturi) este un atac în care o parte terță încearcă să inducă în eroare un sistem de IA conversațional: să îl determine să execute instrucțiuni dăunătoare sau să dezvăluie informații confidențiale. Comenzile rău intenționate pot fi ascunse în pagini web, conținut stocat în cache sau fișiere descărcate pe care modelul le procesează.

Lockdown Mode nu blochează apariția acestor instrucțiuni în conținutul procesat de ChatGPT. În schimb, modul vizează etapa finală a atacului — încercarea de a transmite datele furate către atacator — și blochează canalele de rețea de ieșire prin care aceste date ar putea părăsi rețeaua controlată de OpenAI.


**Ce funcții sunt limitate de acest mod**
Pentru conturile cu Lockdown Mode activat, următoarele capacități sunt dezactivate sau limitate:


******Navigarea web în timp real.** Accesul este limitat doar la conținutul din cache, astfel încât rezultatele căutării pot fi incomplete, indisponibile sau învechite.
******Lucrul cu imagini.** ChatGPT ar putea să nu afișeze imagini în răspunsurile obișnuite și să nu le preia de pe web. Încărcarea propriilor imagini și generarea de imagini rămân disponibile acolo unde funcționează în mod normal.
******Deep Research.** Funcția de cercetare aprofundată este complet dezactivată.
******Agent Mode.** Modul agent este complet dezactivat.
******Rețeaua în Canvas.** Utilizatorul nu poate permite codului generat în Canvas accesul la rețea.
******Încărcarea fișierelor.** ChatGPT nu poate descărca fișiere pentru analiza datelor, însă continuă să lucreze cu documentele pe care utilizatorul le-a încărcat manual.

**Ce NU schimbă Lockdown Mode**
Modul nu afectează memoria, încărcarea fișierelor, posibilitatea de a partaja o conversație sau faptul dacă dialogurile tale pot fi folosite pentru îmbunătățirea modelelor (acest lucru este reglat separat în setările de date). De asemenea, nu restricționează accesul la rețea în Codex.

OpenAI subliniază separat: Lockdown Mode reduce semnificativ riscul exfiltrării datelor prin prompt injection, dar nu garantează că furtul de date este imposibil. Un risc rezidual poate persista din cauza aplicațiilor activate, a combinațiilor neprevăzute de funcționalități sau a unor tehnici de atac noi, încă necunoscute. O instrucțiune dăunătoare ascunsă într-un fișier încărcat poate influența în continuare comportamentul modelului și poate duce la un răspuns eronat.


**Aplicații și conectori în modul Lockdown**
Comportamentul aplicațiilor și al conectorilor depinde de tipul contului. Pentru conturile personale și business self-serve, modul permite conectorii care utilizează date sincronizate, dar blochează accesul la conectorii în timp real și acțiunile de scriere prin intermediul acestora. Unele scenarii conectate — inclusiv Finances în ChatGPT și funcțiile de agent pentru cumpărături — sunt indisponibile în modul Lockdown.

În spațiile de lucru gestionate, aplicațiile, MCP și conectorii sunt controlați de setările spațiului și de modelul de acces bazat pe roluri (RBAC). Modul nu dezactivează automat fiecare aplicație — administratorii sunt sfătuiți să lase disponibile doar aplicațiile și acțiunile de încredere necesare membrilor.


**Cum se activează Lockdown Mode**
Pentru conturile personale și business self-serve eligibile, pașii sunt următorii:


- Deschideți „Settings” (Setări).

- Accesați secțiunea „Security” (Securitate).

- În blocul „Advanced security”, activați „Lockdown Mode”.

- În fereastra de confirmare, apăsați „Turn on”.

Lockdown Mode și Developer Mode nu pot funcționa simultan: activarea unui mod îl dezactivează pe celălalt. Când protecția este activă, deasupra câmpului de introducere apare un mesaj corespunzător. Pentru a dezactiva modul doar pentru o singură conversație, selectați „Manage” în acel mesaj și „Turn off for this chat” — sau utilizați meniul de opțiuni suplimentare.


**Etichetele „Elevated Risk” și contextul larg**
Împreună cu Lockdown Mode, OpenAI a standardizat marcajul „Elevated Risk” (risc ridicat) pentru o serie de funcții din ChatGPT, ChatGPT Atlas și Codex care pot crea riscuri suplimentare. Scopul este de a oferi utilizatorilor aceleași avertismente, indiferent de produsul în care întâlnesc o astfel de posibilitate.

OpenAI numește prompt injection o „problemă de cercetare complexă și avansată” și notează că, în prezent, aceasta nu reprezintă riscul principal, deși impactul său ar putea crește pe măsură ce metodele de atac se complică. Analiștii de securitate atrag atenția asupra unui alt aspect: apariția unui mod separat sugerează indirect că setările tipice ale ChatGPT nu oferă o protecție completă împotriva încercărilor hotărâte de furt de date. Mai multe detalii despre funcție pot fi găsite în [Centrul de Ajutor OpenAI](https://help.openai.com/en/articles/20001061-lockdown-mode).

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/chatgpt-lockdown-mode/?utm_source=responsabil) și a fost tradus în limba română.
