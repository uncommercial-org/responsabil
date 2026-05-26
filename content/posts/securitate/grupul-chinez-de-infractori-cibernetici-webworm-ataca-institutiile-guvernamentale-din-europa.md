---
title: "Grupul chinez de infractori cibernetici Webworm atacă instituțiile guvernamentale din Europa"
date: 2026-05-22
draft: false
description: "ESET avertizează că grupul APT Webworm, legat de China, își extinde atacurile asupra instituțiilor guvernamentale din Belgia, Italia, Polonia, Serbia și Spania folosind noi metode."
categories: ["securitate"]
cover:
  image: "images/cybercalm/grupul-chinez-de-infractori-cibernetici-webworm-ataca-institutiile-guvernamentale-din-europa.jpeg"
  alt: ""
  caption: ""
  relative: false
showToc: true
tocOpen: false
---

Compania ESET avertizează că grupul APT Webworm, legat de China, și-a extins vectorul de atac și acum vizează nu doar țările din Asia, ci și **instituțiile guvernamentale** din Belgia, Italia, Polonia, Serbia și Spania.

Mai exact, de anul trecut, grupul de atacatori folosește backdoor-uri care utilizează **Discord** și **Microsoft Graph API** pentru a se conecta la serverul de comandă. Cercetătorii ESET au decriptat peste 400 de mesaje Discord și au descoperit un server al atacatorilor folosit pentru colectarea de informații despre peste 50 de ținte.

Informațiile i-au condus pe specialiștii ESET și la depozitul Webworm de pe GitHub, care conținea aplicații false, cum ar fi aplicația SoftEther VPN. În fișierul de configurare SoftEther a fost descoperită o adresă IP care corespunde cu o adresă IP cunoscută a Webworm.

> «În cursul analizei, specialiștii ESET au reușit să recupereze comenzile executate de pe server, care permit înțelegerea tehnicilor de obținere a accesului inițial cu ajutorul unui scaner de vulnerabilități open-source, precum și identificarea mai multor obiecte ale atacurilor», explică Erik Howard, cercetător ESET.

Grupul utilizează două noi backdoor-uri: EchoCreep, bazat pe Discord, și GraphWorm, bazat pe Microsoft Graph. Backdoor-ul EchoCreep folosește Discord pentru a descărca fișiere, a trimite rapoarte de activitate și a primi comenzi. GraphWorm folosește Microsoft Graph API pentru a se conecta la serverul de comandă. Cercetătorii ESET au descoperit că cel de-al doilea backdoor utilizează exclusiv stațiile de lucru OneDrive, în special pentru a primi noi sarcini și a încărca informații despre victime.

Deși atacatorii au continuat să folosească soluții proxy existente, aceștia au adăugat și propriile soluții — WormFrp, ChainWorm, SmuxProxy și WormSocket. Având în vedere numărul de instrumente proxy și complexitatea acestora, Webworm **creează potențial o rețea ascunsă mult mai mare pentru a efectua atacuri la scară largă**.

**Grupul continuă, de asemenea, să plaseze fișiere pe GitHub și probabil va continua să o facă**, așa că merită să asigurați o protecție fiabilă a rețelelor corporative împotriva amenințărilor actuale printr-o [abordare cuprinzătoare a securității](https://www.eset.com/ua/business/small-and-medium/).

Mai multe informații detaliate despre grupul Webworm și activitatea sa rău intenționată pot fi găsite [la acest link](https://www.welivesecurity.com/en/eset-research/webworm-new-burrowing-techniques/).

Acest articol a fost publicat anterior pe site-ul [CyberCalm](https://cybercalm.org/webworm-atakuye-derzhavni-ustanovy-v-yevropi/?utm_source=responsabil) și a fost tradus în limba română.
