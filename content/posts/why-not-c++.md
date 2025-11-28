---
date: '2025-11-28T14:47:40+01:00'
draft: true
title: 'Why Not C++'
categories: []
tags: []
cover:
  image: images/
  hiddenInList: false
---

### Perché programmare in C++ oggi è spesso sconveniente

*Scopri perché programmare in C++ oggi è spesso sconveniente. Memory safety, costi di sviluppo e boom delle app desktop Electron.*

---

Quando si parla di linguaggi di programmazione “storici”, C e C++ sono sicuramente i primi a venire in mente a qualsiasi programmatore, occupa sempre un posto speciale in ognuno di noi.

È veloce, potente, capace di tutto. Eppure, oggi più che mai, programmare in C++ può essere una scelta sconveniente. Non perché il linguaggio sia “sbagliato”, ma perché il panorama tecnologico è cambiato totalmente: le esigenze di oggi richiedono sicurezza, sviluppo rapido e un ecosistema più orientato alla produttività che all’ottimizzazione estrema.

In questo articolo voglio esplorare alcuni motivi per cui C++ sta perdendo terreno, soprattutto nel mondo delle applicazioni desktop, e come questo vuoto sia stato riempito da strumenti come Electron — con tutti i suoi pro e contro.

---

## 1. **Il nodo principale: la sicurezza della memoria**

C e C++ concedono grandi poteri… e richiedono grande responsabilità e soprattutto molte competenze. La gestione della memoria è uno dei suoi punti di forza, ma anche il suo tallone d’Achille.

### **Buffer overflow, use-after-free, dangling pointer…**

Sono da anni che programmatori hanno a che vedere con contanti bug fixing critici, quando si programma in C/C++ e facile cadere in errori soprattutto quando mancano certe accortezze.



Sono problemi noti da decenni, e continuano a tormentarci. Qualsiasi programmatore C++ sa che basta una distrazione:

- Un `delete` al posto sbagliato

- Un puntatore non inizializzato

- Un array oltre i limiti

…ed ecco che il programma diventa vulnerabile e mette a rischio la sicurezza del sistema ospitante.

### **Gli strumenti moderni non bastano**

È vero: C++ ha smart pointer, RAII, librerie di alto livello, e gli standard recenti hanno introdotto pratiche più sicure. Ma il linguaggio rimane strutturalmente non memory-safe.

Non esiste un *garbage collector*.  
Non esistono *controlli automatici dei limiti*.  
Non esiste un *modello di memoria intrinsecamente sicuro*.

Certo, puoi programmare “in modo sicuro”, ma richiede disciplina, esperienza, analisi statica e test approfonditi. Ed è qui che i linguaggi moderni prendono il largo.

---

## 2. **Il confronto con i linguaggi memory-safe**

Oggi linguaggi come **Rust**, **Go**, **C#** o **Java** offrono un paradigma molto più protetto. Rust, in particolare, ha dimostrato che è possibile ottenere prestazioni C++ *senza* sacrificare la sicurezza della memoria.

Le aziende stanno iniziando a rendersi conto dei costi del C++:

- patch infinite per problemi di memoria

- vulnerabilità ripetute

- difficoltà nel manutenerlo

- tempi di sviluppo più lunghi

Tant’è che persino Mozilla, Microsoft, Amazon e Google stanno adottando Rust in componenti critici.

Il punto non è che C++ sia “un brutto linguaggio”: è che le sue scelte progettuali non sono più allineate alle priorità moderne.

---

## 3. **Il paradosso delle app desktop moderne**

Mentre i linguaggi nativi lottano con problemi strutturali, il mondo delle app desktop ha preso una direzione completamente diversa: **l’adozione massiva di Electron**.

Electron, nel bene e nel male, ha cambiato il mercato.

### **Perché Electron ha vinto**

- La stessa codebase per Windows, macOS e Linux

- Stack web, quindi milioni di sviluppatori già pronti

- Velocità di prototipazione molto elevata

- Ecosistema enorme

- UI più facile da costruire rispetto a toolkit nativi complessi

E così, applicazioni come VS Code, Discord, Slack e molti altre hanno dominato il panorama desktop… pur essendo essenzialmente browser mascherati da app.

### **Il problema: Electron è pesante**

E questo è l’altro lato del paradosso.

Applicazioni che potrebbero pesare pochi megabyte diventano facilmente:

- centinaia di MB sul disco

- decine o centinaia di MB di RAM

- lente a partire

- voraci di risorse

Paradossalmente, molti sviluppatori evitano C++ perché difficile e rischioso… e finiscono con l'usare un framework che spreca risorse per evitare i problemi della memoria non sicura.

---

## 4. **C++ può ancora avere un ruolo?**

Assolutamente sì, soprattutto dove servono:

- prestazioni estreme

- controllo totale del sistema

- latenza ridotta

- compatibilità con codice storico

- sviluppo di motori grafici, giochi, sistemi embedded, driver

Ma per molte applicazioni moderne — soprattutto desktop — il costo di usarlo è spesso superiore ai benefici.

La tendenza attuale è chiara:

- i nuovi progetti lo usano sempre meno

- l’industria si sposta verso linguaggi memory-safe

- il mondo consumer preferisce applicazioni cross-platform veloci da sviluppare

C++ svolgerà sempre un ruolo importante, ma non è più il linguaggio “universale” di una volta.

---

## **Conclusione**

Programmare in C++ oggi non è “sbagliato”, ma spesso diventa sconveniente quando si considerano sicurezza, tempi di sviluppo e gestione della memoria. Se da un lato abbiamo un linguaggio potente ma potenzialmente pericoloso, dall'altro abbiamo framework come Electron che risolvono i problemi di produttività a scapito dell’efficienza.

Il futuro probabilmente troverà un equilibrio: linguaggi come Rust si faranno strada, e i toolkit nativi moderni torneranno ad essere competitivi. Nel frattempo, dobbiamo accettare che l’evoluzione del software passa anche attraverso compromessi: non sempre i più eleganti, ma quelli che permettono di costruire prodotti più rapidamente e in modo più sicuro.

In fondo, la programmazione non è solo questione di linguaggi: è questione di scelte, contesto ed esigenze reali.
