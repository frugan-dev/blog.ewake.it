---
layout: post
title: Supporto a TLS 1.3 e connessioni STARTTLS deprecate
---


Un paio di settimane fa, con l'occasione della sostituzione dei proxy mail, abbiamo dovuto aggiornare i protocolli TLS della **posta in uscita**, introducendo il supporto a TLS 1.3, e deprecando il supporto a TLS inferiore o uguale a 1.1.  
Inoltre abbiamo predisposto **entro fine anno** l'abbandono degli accessi STARTTLS sulle porte 143 (IMAP), 110 (POP3) e 587 (SMTP), in quanto considerati non più sicuri <a href="https://www.rfc-editor.org/rfc/rfc8314#section-3.3">https://www.rfc-editor.org/rfc/rfc8314#section-3.3</a>.

Nei **prossimi giorni/settimane** procederemo ad applicare gli stessi aggiornamenti ai protocolli TLS anche sulla posta in entrata, scaglionando gradualmente le modifiche per tutti i clienti.

### Che cosa cambia per te?

Se sei connesso via SSL/TLS sulle porte 993 (IMAP), 995 (POP3) o 465 (SMTP), non devi cambiare alcuna impostazione.

Se invece sei connesso via STARTTLS sulle porte 143 (IMAP), 110 (POP3) o 587 (SMTP), allora ti invitiamo **entro fine anno** a passare a SSL/TLS sulle rispettive porte 993 (IMAP), 995 (POP3) e 465 (SMTP).

### Sono possibili alcuni disguidi?

Il nuovo protocollo TLS 1.3, pur essendo più sicuro e veloce <a href="https://kinsta.com/it/blog/tls-1-3/">https://kinsta.com/it/blog/tls-1-3/</a>, è però anche più restrittivo in termini di compatibilità con i dispositivi/programmi in uso, e richiede pertanto l'utilizzo di client mail aggiornati, come ad es. Thunderbird (consigliato), Outlook, Mail (iOS), ecc.  
Purtroppo però anche l'utilizzo di dispositivi/programmi aggiornati, non sempre scongiura alcuni piccoli disguidi, nella maggior parte dei casi comunque di lieve entità.  
Di seguito le casistiche più comuni:

Problema:  
**Il client di posta richiede nuovamente l'inserimento della password.**  
Soluzione:  
Quando il client la richiede, reinserire la stessa password sia per la posta in entrata che per quella in uscita, avendo cura di spuntare "memorizza la password".  
Attenzione a non copiare spazi vuoti durante il copia-incolla.

Problema:  
**Il client di posta scarica nuovamente le email già precedentemente scaricate.**  
Soluzione:  
Questo problema riguarda solo il protocollo POP3, e può accadere con differenti client di posta (ad es. Thunderbird <a href="http://kb.mozillazine.org/Duplicate_messages_received">http://kb.mozillazine.org/Duplicate_messages_received</a>, Outlook <a href="https://www.emaildoctor.org/blog/why-outlook-is-downloading-duplicate-emails/">https://www.emaildoctor.org/blog/why-outlook-is-downloading-duplicate-emails/</a>).  
In pratica ci si ritrova con le email duplicate nella posta in arrivo, generalmente solo quelle degli ultimi 30 o più giorni.  
Nella maggior parte dei casi è sufficiente ordinarle per data, in modo da procedere poi agevolmente alla cancellazione dei duplicati.

Problema:  
**Il client di posta non riesce più a scaricare o ad inviare le mail.**  
Soluzione:  
Se utilizzi client mail obsoleti (ad es. Windows Live Mail), è possibile che nei prossimi giorni/settimane tu non riesca più a connetterti ai server di posta.  
Per questioni di sicurezza non possiamo consentire delle eccezioni in tal senso, in quanto il loro impatto globale metterebbe a rischio anche altri utenti non interessati dal problema.  
Se rientri in questa ristretta casistica, ti invitiamo a fare un upgrade dei tuoi dispositivi/programmi in uso, e a contattarci ai recapiti in calce per informazioni o assistenza.

### Webmail

Ricordiamo inoltre che in caso di urgenza è sempre disponibile online l'accesso tramite webmail all'indirizzo http://webmail.DOMINIO.TLD (sostituire DOMINIO.TLD con il proprio nome a dominio).

Scusandoci in anticipo per eventuali disagi, rimaniamo a disposizione per informazioni ed assistenza ai [seguenti recapiti]({{ site.mainurl }}).
