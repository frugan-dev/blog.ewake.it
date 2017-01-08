---
layout: post
title: Utilizzo sperimentale di Google Analytics tramite Google PageSpeed
---

Grazie al consolidato utilizzo del [modulo PageSpeed](https://developers.google.com/speed/pagespeed/module/) di Google, [EWake]({{ site.mainurl }}) sta ora sperimentando la funzionalità di inserimento del codice di Google Analytics direttamente nelle pagine tramite il filtro [insert_ga](https://developers.google.com/speed/pagespeed/module/filter-insert-ga).

Attualmente la soluzione sembra avere alcune problematiche solo con le pagine dinamiche in PHP in modalità PHP-FPM; ciò nonostante [EWake]({{ site.mainurl }}) ha deciso di renderla comunque operativa per tutti i clienti che verranno prossimamente aggiornati al [nuovo pannello di gestione dei servizi cloud]({{ site.baseurl }}{% post_url 2016-12-05-nuova-interfaccia-del-pannello-di-gestione-dei-servizi-cloud %}): la possibilità infatti di utilizzo del filtro con PHP in modalità FastCGI garantisce comunque la funzionalità del servizio di tracking.

Si avvisano quindi tutti i clienti interessati della **presenza del codice ID di Google Analytics all'interno del file _.htaccess_**, come indicato di seguito:

```text
<IfModule pagespeed_module>
...
ModPagespeedAnalyticsID UA-12345678-1
...
</IfModule>
```
Una copia originale del file _.htaccess_ di default è anche disponibile [al seguente indirizzo]({{ site.publicurl }}).

Analogamente, per evitare il tracciamento delle pagine di amministrazione dei CMS, all'interno delle cartelle di amministrazione sarà presente un _.htaccess_ con le seguenti direttive:

```text
<IfModule pagespeed_module>
...
ModPagespeedDisableFilters insert_ga
...
</IfModule>
```

**[EWake]({{ site.mainurl }}) non si ritiene pertanto responsabile del mancato tracciamento delle statistiche mensili**, nei casi in cui:

- il codice indicato (`ModPagespeedAnalyticsID <Analytics ID>`) venisse rimosso dal file _.htaccess_ o commentato direttamente dai clienti o da chi per essi
- venisse disabilitato il filtro [insert_ga](https://developers.google.com/speed/pagespeed/module/filter-insert-ga) via _.htaccess_ (`ModPagespeedDisableFilters insert_ga`)
- venisse disabilitato il modulo PageSpeed via _.htaccess_ (`ModPagespeed off`)
- venisse abilitata la modalità PHP-FPM

Sperando nel frattempo in un prossimo aggiornamento del modulo che risolva la problematica evidenziata, si rimanda alla [documentazione ufficiale](https://developers.google.com/speed/pagespeed/module/), a quella di [supporto EWake]({{ site.supporturl }}) e ai [seguenti recapiti]({{ site.mainurl }}) per maggiori informazioni. 