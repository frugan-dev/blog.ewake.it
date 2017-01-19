---
layout: post
title: "Nuova vulnerabilità su Magento: componente email Zend Framework"
---

Una nuova vulnerabilità è stata trovata sul componente email di Zend Framework 1 e 2 che viene utilizzato da tutti i software Magento 1 e 2 e altre soluzioni PHP. 
Questa vulnerabilità può portare ad un attacco di esecuzione di codice remoto se il server utilizza Sendmail come sistema per l’invio della posta.

Anche se non ci sono stati ancora attacchi da questo tipo di vulnerabilità, il rischio è molto elevato, 
ma nelle prossime settimane verrà rilasciata una patch ufficiale di sicurezza.

Nel frattempo è possibile controllare se il proprio ecommerce è vulnerabile a questa falla sulla sicurezza andando alle impostazioni di sistema:

**Magento 1:** _Sistema -> Configurazione -> Avanzate -> Sistema -> Mail Sending Settings -> Set Return-Path_

**Magento 2:** _Stores -> Configurazione -> Avanzate -> Sistema -> Mail Sending Settings -> Set Return-Path_

Se "Set Return-Path" è impostato su "Sì" significa che si è vulnerabili a questo tipo di problema; e per risolverlo temporaneamente è sufficiente impostare su "No" e aggiornare la cache.

Questo il post ufficiale <a href="https://magento.com/security/news/new-zend-framework-1-security-vulnerability" target="_blank">https://magento.com/security/news/new-zend-framework-1-security-vulnerability</a>.

Per maggiori informazioni contattaci ai [seguenti recapiti]({{ site.mainurl }}). 