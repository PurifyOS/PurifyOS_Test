  Copyright (c)  2017  Ernesto Castellotti.
  
   Permission is granted to copy, distribute and/or modify this document
   under the terms of the GNU Free Documentation License, Version 1.2
   or any later version published by the Free Software Foundation;
   with no Invariant Sections, no Front-Cover Texts, and no Back-Cover
   Texts.  
   A copy of the license is included in the section entitled "LICENSE".
   
   
   ## **Technical TEST**
## **PurifyOS Stable - build #2**
&nbsp;
#  Languages ​​available

 - **[Italiano](#it)**
<a name="it">
&nbsp;
&nbsp;

![magisk_logo](http://i.imgur.com/UT8TYbk.png)

# Dati tecnici
  - Dispositivo: Oneplus 3 (A3003 3fce319)
  - Android: 7.1.1
  - Versione PurifyOS: Stable - build #2
  - Recovery: TWRP 3.1.1 Oneplus3 by PurifyOS
  - Versione Kernel Linux: 3.18.32-perf+
  - Versione Magisk: 13.3
  - Patch di sicurezza Android: Maggio 2017
  - Operatore: H3G Italy (22299)
  - Memoria RAM: 6GB LPDDR4, 52,67 GB effettiva
  - Spazio archiviazione: 64GB UFS 2.0 dichiarati, 52,67 GB totale effettivi (8,92 GB usati)
  - SoC: Snapdragon 820 (msm8996)
  - CPU: Quad Core, Kryo: 2x 2.2 GHz, 2x 1.6 GHz
  - Architettura CPU: 64 bit ARMv8-A (arm64-v8a, armeabi-v7a, armeabi)
  - GPU: Adreno 530
  - Batteria: Li-Ion 3000 mAh
  - Schermo: 1080x1920 (401 PPI) Optic AMOLED 60 Hz (Samsung s6e3fa3 1080p cmd mode dsi panel)
  - Versione OpenGL: ES 3.2 V@145.0 (GIT@I9c435c2712)
  - App extra installate non incluse in PurifyOS: Plus Messager, AIDA64, GrooVe IP)
 
# Stato telefono
 - System: formattato prima dell'installazione
 - Data: formattato prima dell'installazione
 - Cache: formattato prima dell'installazione
 - Dalvik-cache: formattato prima dell'installazione


# Tipo di TEST: TEST tecnico
## Test effettuati VIF (Funzioni veramente importanti):

  - Avvio del telefono
  - Spegnimento telefono
  - Configurazione guidata iniziale
  - Ricezione ed invio di chiamate (incluso SOS)
  - Ricezione ed invio di SMS
  - Ricezione ed invio di chiamate in roaming
  - Rete mobili (anche in roaming)
  - WiFi
  - Ricarica batteria
  - Rotazione schermo
  - GPS
  - Bluetouch
  - Riproduzione audio (Speaker interno, periferica collegata tramite Jack, periferica bluetouch)
  
## Test effettuati IF (Funzioni importanti):
 - Sblocco tramite impronta digitale (4 diti)
 - Mappatura azioni tasti hardware
 - Gesture schermo 
 - TEST stabilita soggettiva (rapido: 1/2 h)
 - Controllo luminosità schermo
 - TEST temperatura CPU, GPU, Batteria (rapido: 2h)
 - Navigazione Internet via Chrome
 - Download file via Chrome
 - TEST funzioni PurifyOS
 - TEST fotocamera completo
 - Connessione a Google Account
 - Download a installazione app tramite Google Play Store
 - TEST generico app di sistema
 - Registrazione audio vocale
 
## Test effettuati NIF (Funzioni non importanti):
 - Applicazione profilo AKT 
 - Applicazione hosts AdAway
 - Download e installazione app tramite F-Droid
 - Editing foto tramite galleria
 - Equalizzazione audio con AudioFX (incluso in PurifyOS)
 - Registrazione schermo 
 - File manager MiXplorer
 - Riproduzione video Youtube tramite NewPipe (incluso in PurifyOS)
 - Sveglia
 - Applicazione temi 
 
# TEST FALLITI

## Test VIF falliti
 - Problema minore nella configurazione guidata iniziale #1

## Test IF falliti
 - Nessuno

## Test NIF falliti
 - Problema grave nella installazione app tramite F-Droid #2
 - Scomodità iniziale nella registrazione schermo #3

# **Problemi scoperti**
# Problema #1
## Sintomi:
Durante la configurazione iniziale le app "PurifyOS Impostazioni" e "AKTApp" chiedono i permessi di root per eseguire gli script all'avvio, questo può causare una negazione dei permessi alle app citate
## Soluzioni possibili da implementare in PurifyOS:
 - Sconosciute
## Soluzione che l'utente può eseguire per risolvere temporaneamente il problema:
 - Controllare dopo la configurazione i permessi delle app citate da Magisk Manager e in caso di permessi negati abilitarli manualmente

# Problema #2
## Sintomi:
F-Droid fallisce lo scaricamento dei repository se installata in /system (default in PurifyOS)
## Soluzioni possibili da implementare in PurifyOS:
 - Installare l'app in /data
## Soluzione che l'utente può eseguire per risolvere temporaneamente il problema:
 - Scaricare l'apk di F-Droid e installarlo manualmente, durata tecnica 1 minuto
# Problema #3
## Sintomi:
Il registratore di schermo si rifiuta di iniziare la registrazione per mancanza di permessi 
## Soluzioni possibili da implementare in PurifyOS:
 - Aggiungere i permessi necessari al registratore, durata tecnica 10 minuti
## Soluzione che l'utente può eseguire per risolvere temporaneamente il problema:
 - Abilitare manualmente tutti i permessi
</a>
