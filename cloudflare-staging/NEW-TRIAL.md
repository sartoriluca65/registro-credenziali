# Nuova prova separata — 7 novembre 2026

SYNC_SPACE=trial-2026-11-07 seleziona un nuovo namespace server per ogni identità Cloudflare Access verificata. Identità originali, righe D1, oggetti R2, chiavi e copie locali precedenti non vengono cancellati né aggiornati. Il browser apre una generazione locale distinta perché cambia l'identificativo derivato. Il nome dell'app resta registro-credenziali, con comportamento e AAD invariati nella nuova prova. Senza SYNC_SPACE il derivato originale resta esattamente invariato.

Test sintetici: firma e identità JWT, derivazione deterministica, isolamento fra vecchia e nuova prova, rifiuto richieste da schede precedenti, permanenza delle due revisioni dopo le scritture, lettura della vecchia copia e rifiuto configurazioni invalide; suite 13/13 superata.

Ricaricare la pagina sui due dispositivi. Creare la chiave solo sul primo, conservarla e usare la stessa sul secondo. Non riutilizzare schede aperte prima della modifica. Vecchi archivi conservati; il rollback del solo SYNC_SPACE li rende nuovamente selezionabili, sempre con la loro chiave originale. Nessun dato reale è stato letto/importato per questa modifica.
