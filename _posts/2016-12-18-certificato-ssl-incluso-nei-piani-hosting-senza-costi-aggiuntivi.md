---
layout: post
title: Certificato SSL incluso nei piani hosting senza costi aggiuntivi
---

Da oggi in poi in tutti i piani hosting [EWake]({{ site.mainurl }}) è disponibile **senza costi aggiuntivi** un certificato SSL del tipo _Let's Encrypt_ con algoritmo hash SHA-256 e rinnovo automatico ogni 90 giorni.

Per attivarlo è sufficiente spuntare l'opzione **Let's Encrypt** nelle impostazioni del [nuovo pannello hosting EWake]({{ site.baseurl }}{% post_url 2016-12-05-nuova-interfaccia-del-pannello-hosting %}) e configurare opportunamente la propria applicazione affinché supporti il protocollo HTTPS.
Tale opzione è disponibile per tutti i domini e relativi sottodomini, e mantiene distinti i certificati fra i domini e i sottodomini, rendendo quindi irrilevante la necessità del supporto wildcard.

Per i clienti che necessitano comunque di opzioni aggiuntive, quali ad es. 

- autenticazione client S/MIME
- supporto wildcard
- garanzia assicurativa > US $ 10,000
- algoritmo hash SHA-384, SHA-512
- completo supporto dei browser

sono disponibili anche dei certificati SSL del tipo _StartCom Class 2_ o superiore a fronte di un piccolo costo aggiuntivo annuale.

[comment]: # A partire dal primo rinnovo si può liberamente scegliere di mantenere oppure no il certificato a fronte di un piccolo costo aggiuntivo annuale.

I certificati SSL sono importanti per la sicurezza e l'<a href="https://webmasters.googleblog.com/2014/08/https-as-ranking-signal.html" target="_blank">indicizzazione</a> del tuo dominio.
Con l'attivazione di questo protocollo, tutti i dati trasferiti tra una pagina web e un utente finale vengono cifrati e non possono essere intercettati da terzi non autorizzati ad accedere ad essi.
Si tratta di una funzionalità particolarmente interessante nella gestione e nell'utilizzo delle piattaforme di e-commerce che prevedono il passaggio di dati spesso strettamente riservati, inclusi quelli riguardanti transazioni monetarie.

A chi utilizza **Wordpress** consigliamo l'installazione del plugin <a href="https://it.wordpress.org/plugins/better-wp-security/" target="_blank">iThemes Security</a> e l'attivazione della relativa opzione **SSL**.

A chi utilizza **Joomla!** consigliamo invece la <a href="https://www.gavick.com/documentation/joomla/how-to-use-ssl-in-a-joomla-site" target="_blank">seguente guida</a>.

Mentre chi utilizza **Drupal** può trovare maggiori istruzioni sul <a href="https://www.drupal.org/https-information" target="_blank">sito ufficiale</a>.

Per maggiori informazioni e supporto contattaci ai [seguenti recapiti]({{ site.mainurl }}).