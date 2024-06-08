---
layout: blog
title: Datu uzglabāšana & backup
date: 2024-06-08 17:28:45
tags: [lifestyle]
---

## Syncthing

Ilgtermiņa failu uzturēšanai izmantojam:
- [Syncthing](https://syncthing.net/) sinhronizēšanu
- Rūķi kā starpnieku starp ierīcēm un cieto disku

Sinhronizēšana notiek visos personīgajos telefonos un datoros, kas tiek izmantoti ikdienā.

Syncthing ir diezgan gudrs, tāpēc pieļaujami dažādi sinhronizēšanas virzieni.


## PARA

Failu sistēmas formāts aizgūts no Clearer Thinking raidieraksta epizodes ar Tiago Forte par "ārējo galvu" [How to build your second brain](https://podcast.clearerthinking.org/episode/144/tiago-forte-how-to-build-your-second-brain)

Ārējās galvas struktūrā visi faili tiek sadalīti 4 grupās PARA:
- **Projects**: aktīvi projekti ar sākumu un beigām
- **Areas**: mūžīgie projekti (veselība, uzņēmums, ...)
- **Resources**: objekti, ko plāno izmantot nākotnes projektos (grāmatas, koda fragmenti...)
- **Archive**: projekti, kas beigušies un resursi, kas šobrīd vairs nav aktuāli, lai nav jāmet pavisam miskastē

## Īstenošana

Mūsu mērķis ir:
- sastrukturizēt visu digitālo dzīvi pēc ārējās galvas principiem;
- izveidot funkcionālu sinhronizēšanu ar telefoniem (ko ir grūti labi izdarīt);
- atbrīvoties no lēni mirstošā [Keybase](https://keybase.io/), kurš šobrīd vēl pilda svarīgākās funkcijas.

Failu strukturizēšanai izmantojam PARA principu un pievienojam vēl citas grupas atkarībā no personīgajiem ieradumiem. Piemēri ar 2 grupām, ko izmantojam abi:
- **Sentimental**: vieta atmiņu objektiem ar sentimentālu vērtību (bildes, video, ...)
- **Keys**: svarīgākie dokumenti (atslēgu faili). Tikai privātām vajadzībām

![Kalvja mapju struktūra](/images/backup_folders.png)

Mapju struktūru kārtojam primāri pēc piederības:
- Kalniņi
- Kalvis
- Rota

Katrā piederībā atrodas pilna mapju struktūra un faili tiek sinhronizēti tikai ar iesaistītajām pusēm.

> Piemēram, Kalvim nav pieeja Rotas personīgajiem failiem un otrādi, bet abiem ir pilna pieeja Kalniņu failiem.

- Telefoniem pieeja tikai atslēgu mapei, jo ierobežota atmiņa un atvēršanas iespējas.
- Projektus, kuriem ir savi Git, nedublējam - tur jau tiek izmantota labāka versiju sistēma.

