+++
categories = ["Hugo"]
date = "2023-01-20"
description = "Perchè contribuire ad un progetto open source?"
featured = "pic01.jpg"
featuredalt = ""
featuredpath = "date"
linktitle = ""
title = "Perchè contribuire ad un progetto open source?"
slug = "Perchè contribuire ad un progetto open source?"
type = "post"
+++

## Intro
Hugo è un framework leggero e veloce per creare siti statici come questo!
Se necessiti di una piattaforma per compilare un sito Hugo e avere un deploy automatizzato in cloud, Netlify potrebbe essere la scelta giusta per te. Sono rimasto immediatamente affascinato quando ho visto che Netlify ti da la possibilità di velocizzare e prendere il controllo del tuo processo di rilascio. Inoltre si hanno a disposizione pipline configurabili e anche molti altri servizi serverless.

### La mia prima pull request in un progetto open source
La mia prima pull request l'ho fatta per gestire l'animazione del logo per questo tema Hugo.
Se si cambia pagina il percorso mostrato cambia di conseguenza. dopo alcuni giorni la PR è stata accettata ed è stato fatto merge in master.


Un po del codice javascript necessario per concatenare l'url path al testo contenuto nel logo:
(l'evento `window.onload` viene scatenato al caricamento di una nuova window.)
```
const language = document.getElementsByTagName('html')[0].lang;
const logo = document.querySelector(".logo__pathname");
if(logo){
  window.onload = () => {
    let path = window.location.pathname.substring(1);
    path = path.replace(language+'/','')
    logo.textContent += path.substring(0,path.indexOf('/'));
  };
}
```

### Perchè contribuire ad un progetto open source?
Quando ho approcciato il progetto di questo sito mi sono domandato se fosse meglio un tema già fatto o partire da zero prendendo qualche spunto.
In realtà ho scoperto che la miglior soluzione è certamente usare un tema Hugo già fatto ma contribuire al progetto open source.
Sicuramente questa è una opportunità che dona molto valore a ciò che si stà facendo. Sono entusiasta di aver contribuito ad un progetto open, sicuramente è stata la scelta migliore. Ho imparato l'importanza di condividere nuove funzionalità che molte persone potranno usare in futuro. Mi sono convinto che l'open source è il giusto approccio per creare progetti robusti. Spero di continuare a portare valore nel mondo open source.