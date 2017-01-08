---
layout: post
title: "Avviso di sicurezza: vulnerabilità di PHPMailer"
---

Si avvisano i gentili clienti che è stata resa nota una nuova vulnerabilità di sicurezza critica a carico dell'applicazione web [PHPmailer](https://github.com/PHPMailer/PHPMailer) fino alla versione 5.2.17.
 
Tale vulnerabilità, se sfruttata, permette ad un eventuale hacker l'esecuzione di codice arbitrario all'interno dello spazio del dominio con possibile compromissione del sito web e invio di email di spam dagli script in uso nel sito.

**Anche tutti i siti realizzati con Wordpress, Joomla e Drupal sono affetti da questa vulnerabilità.**

Per **Wordpress** non esiste però ancora una patch o aggiornamento ufficiale del core che risolva il problema.  
Con **Joomla** invece il problema è risolvibile con l'[aggiornamento alla versione 3.7](https://developer.joomla.org/security-centre/668-20161205-phpmailer-security-advisory.html).  
Infine per **Drupal** esiste una [patch ufficiale](https://www.drupal.org/psa-2016-004).

[EWake]({{ site.mainurl }}) provvederà, dove possibile, ad aggiornare l'applicativo alla [versione 5.2.21 appena rilasciata](https://github.com/PHPMailer/PHPMailer/blob/master/changelog.md), con la quale tale problema è stato risolto, a tutti i siti dei clienti che verranno prossimamente trasferiti sul [nuovo pannello di gestione dei servizi cloud]({{ site.baseurl }}{% post_url 2016-12-05-nuova-interfaccia-del-pannello-di-gestione-dei-servizi-cloud %}).  
Nel frattempo però si invitano i clienti non ancora trasferiti a provvedere autonomamente all'aggiornamento dell'applicativo [PHPmailer](https://github.com/PHPMailer/PHPMailer).

Di seguito alcuni articoli sull'argomento:

- <a href="http://thehackernews.com/2016/12/phpmailer-security.html" target="_blank">http://thehackernews.com/2016/12/phpmailer-security.html</a>
- <a href="https://www.wordfence.com/blog/2016/12/phpmailer-vulnerability/" target="_blank">https://www.wordfence.com/blog/2016/12/phpmailer-vulnerability/</a>
- <a href="https://developer.joomla.org/security-centre/668-20161205-phpmailer-security-advisory.html" target="_blank">https://developer.joomla.org/security-centre/668-20161205-phpmailer-security-advisory.html</a>
- <a href="http://hackaday.com/2016/12/25/santa-knows-if-your-contact-form-uses-phpmailer-5-2-18/" target="_blank">http://hackaday.com/2016/12/25/santa-knows-if-your-contact-form-uses-phpmailer-5-2-18/</a>
- <a href="https://www.drupal.org/psa-2016-004" target="_blank">https://www.drupal.org/psa-2016-004</a>
- <a href="https://www.mydropwizard.com/blog/drupal-6-workaround-highly-critical-vulnerability-phpmailer" target="_blank">https://www.mydropwizard.com/blog/drupal-6-workaround-highly-critical-vulnerability-phpmailer</a>


Per maggiori informazioni contattaci ai [seguenti recapiti]({{ site.mainurl }}).
