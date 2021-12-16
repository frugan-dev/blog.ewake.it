---
layout: post
title: Dismissione STARTTLS dal 1° Gennaio 2022
---


Come da comunicazione precedente del 23 Ottobre 2021 "[Upgrade a TLS 1.3 e connessioni STARTTLS deprecate]({{ site.url }}/2021/10/22/upgrade-a-tls-1-3-e-connessioni-starttls-deprecate.html)", ti ricordiamo che dal **1° Gennaio 2022** verranno dismessi gli accessi STARTTLS sulle porte 143 (IMAP), 110 (POP3) e 587 (SMTP), in quanto considerati non più sicuri <a href="https://www.rfc-editor.org/rfc/rfc8314#section-3.3">https://www.rfc-editor.org/rfc/rfc8314#section-3.3</a>.

### Che cosa cambia per te?

Se sei connesso via SSL/TLS sulle porte 993 (IMAP), 995 (POP3) o 465 (SMTP), non devi cambiare alcuna impostazione.

Se invece sei connesso via STARTTLS sulle porte 143 (IMAP), 110 (POP3) o 587 (SMTP), allora ti invitiamo **entro fine anno** a passare a SSL/TLS sulle rispettive porte 993 (IMAP), 995 (POP3) e 465 (SMTP).


### Webmail

Ricordiamo che in caso di urgenza è sempre disponibile online l'accesso tramite webmail all'indirizzo <a href="http://webmail.ewake.it">http://webmail.ewake.it</a>.

Scusandoci in anticipo per eventuali disagi, rimaniamo a disposizione per informazioni ed assistenza ai [seguenti recapiti]({{ site.mainurl }}).
