Annotation Scheme
=================

The annotation scheme for this linguistic corpus follows specific rules to ensure consistency and accuracy in annotating contractual texts. Segmentation is crucial, with texts divided into clauses, subparagraphs, or sub-clauses using periods as the textual division marker. Annotators are assigned halves of the dataset and review each other's annotations to maintain quality. Only text directly related to the contract's subject matter and affecting the parties' positions is annotated, ensuring relevance. Annotation strings are separated following punctuation for clarity and to ensure coherent meanings. Labels denote various contract elements, with the most generic chosen if there's uncertainty. The aim is to provide precise annotations while only revealing the domain to the machine, maintaining confidentiality.

Annotation rules:
=================

1.  Segmentation: texts are divided into clauses, subparagraphs, or sub-clauses for segmentation, utilizing "periods" as the textual division marker;

2.  Annotation: strings of words indicating the appropriate label should be separated following punctuation (e.g., period to period, semicolon to semicolon, comma to comma). Each string should convey a complete sense, except for bulleted points of a list, where the introduction sentence preceding it completes the meaning;

3.  Review: each annotator is responsible for annotating half of the dataset, followed by a review of the other annotator's annotations;

4.  Relevance: the annotation process refers to provisions that do create or amend the subjective rights of the parties  and therefore there are legal consequences associated with the textual wording of the clause;

5.  Labels: the following labels comprehend both positive and negative actions, whether they define a legal provision or exclude its application within the context of the contract;

6.  Punctuation: the annotated reference text must include the article (if any) and should be free of bulleted lists and numbers. Initial or final punctuation of the annotation should be omitted;

7.  Indecision: if an annotator is doubtful between two labels applicable to the reference text, but certain on the category, the most generic label is chosen. At any rate, labels are tools to help the annotator to be more precise, however only the domain is provided to the machine.

8.  Annotation scope: a generic annotation (e.g., termination_clause) can encompass a specific annotation (e.g., termination_term) within the same string.

9.  Examples: examples (e.g.) within the contract clause shall not be annotated;

10. Links: links are not annotated unless they are necessary to complete the sentence's meaning.

Labels
======

The following 33 labels of the coding scheme have been manually clustered into 14 categories, covering the main legal aspects characterizing the Terms-and-Conditions contracts:

1.  Party;

2.  Date;

3.  Competence;

4.  Remedy;

5.  Termination;

6.  Term;

7.  Intellectual Property;

8.  License;

9.  Liability;

10. Warranty;

11. Acceptance;

12. Amendment;

13. Audit;

14. Data Protection.

PARTY
-----

-   Party\
    Definition: the two or more parties who signed the contract (e.g., names of persons or entities)\
    Category: party

Examples:

"Se l'utente risiede nel Nord America, la sua relazione è con Adobe Systems Incorporated" (Adobe)

"Adobe Systems Incorporated: 345 Park Avenue, San Jose, California 95110-2704" (Adobe)

-   Party_characteristics

Definition: a clause which limits the access to a service or product, or the ability to enter into a contract depending on characteristics of the contracting party (e.g., age, criminal records, natural or legal person).\
Category: party

Examples:

"per utilizzare i nostri Servizi devi avere almeno 13 anni" (Dropbox)

"l'utente deve essere idoneo all'uso dei servizi EA per i quali si effettua la registrazione ed essere residente in un paese in cui è permesso l'utilizzo dei servizi EA" (EA)

"Diventare membro non richiede alcun costo di iscrizione e l'unica condizione è completare due (2) soggiorni nell'arco di due (2) anni" (Booking)

"Se l'utente ha un'età compresa tra quella minima richiesta e 18 anni (o la maggiore età nel paese di residenza), è necessario rivedere il presente Accordo insieme a genitori o tutori legali" (EA)

-   Third_beneficiary\
    Definition: a clause establishing that a non-contracting party is the beneficiary of all or some clauses of the contract and, as a consequence, can enforce its rights towards a contracting party.

Category: party

Examples:

"L'utente può nominare un soggetto (definito contatto erede) per la gestione del suo account reso commemorativo" (Facebook)

"Noi possiamo trasferire a terzi i nostri diritti previsti dalle presenti condizioni" (Adobe)

-   Party_change\
    Definition: a clause establishing whether the consent or notification of a party is necessary if the contract is transferred to a third party. 

Category: party

Examples:

"L'utente non può cedere o altrimenti trasferire queste condizioni o i diritti e gli obblighi da esse previsti, in tutto o in parte, senza il nostro consenso scritto" (Adobe)

DATE
----

-   Agreement_date\
    Definition: the date of conclusion of the contract (e.g., gg/mm/aaaa)\
    Category: date

Examples:

"Ultima modifica: 30 aprile 2014" (Google)

-   Effect_date\
    Definition: the date from which the contract becomes effective (e.g., gg/mm/aaaa)

Category: date

Examples:

"In vigore dall'1 maggio 2018" (Pinterest)

"Data di validità: 25 maggio 2018" (Dropbox)

"30 giorni dopo la pubblicazione" (EA)

Notes:

-   INCLUDED negative instances of time "non prima di 30 giorni successivi alla data di notifica" (Dropbox)

-   Expiration_date

Definition: the date expiration of the contract (e.g., gg/mm/aaaa or indefinite)\
Category: date

Examples:\
"al 31/03/2024" in "Il presente contratto decorre dal 1/03/2024 al 31/03/2024 e non si rinnova alla scadenza"

COMPETENCE
----------

-   Contract_hierarchy\
    Definition: a clause defining the hierarchy between the contract and other contracts.\
    Category: competence

Examples:

"Qualora l'utente abbia stipulato con noi un altro contratto riguardante il Software in questione, le condizioni di tale contratto prevarranno in caso di conflitto con le presenti" (Adobe)

"la versione in lingua inglese farà fede in caso di controversie" (Dropbox)

Notes:

-   internal hierarchies between clauses within the same contract are NOT INCLUDED:

Example: "I seguenti termini si applicano all'Utente e sostituiscono i termini in conflitto nel presente Contratto" (Grindr)

-   Applicable_law\
    Definition: it defines the legal framework or set of laws that govern the interpretation, enforcement, and resolution of disputes related to a particular contract. This label indicates the jurisdiction whose laws are applicable to the contract and any disputes that may arise from it.\
    Category: competence

Examples:

"Se l'utente risiede nel Nord America, la sua relazione è con Adobe Systems Incorporated, una società statunitense, e il Software è disciplinato dalle leggi della California (USA)" (Adobe)

"Per i consumatori in Nuova Zelanda che hanno il Software in concessione per uso personale, domestico o familiare (non per scopi commerciali), il presente contratto è soggetto al Consumer Guarantees Act" (Adobe)

-   ADR\
    Definition: a clause establishing the resolution of controversies through alternative dispute resolution (ADR) (e.g., arbitration, mediation)\
    category: competence

Examples:

"L'utente e Dropbox accettano di risolvere qualsiasi reclamo relativo ai presenti Termini o Servizi tramite arbitrato finale e vincolante condotto da un singolo arbitro" (Dropbox)

Notes:

-   any indications about legal fees are INCLUDED:\
    Example: "Se l'arbitro ritiene che tali costi siano eccessivi o se l'utente invia a EA, all'indirizzo della Notifica di Controversia, una comunicazione in cui dichiara di non essere in grado di pagare le spese necessarie all'avvio di un arbitrato, EA pagherà tutte le spese connesse all'arbitrato" (EA)

-   Appointed_court\
    Definition: a clause establishing the competent court for disputes linked to the contract.\
    Category: competence

Examples:

"L'utente e Dropbox accettano che qualsiasi procedimento giudiziario per risolvere i reclami relativi ai presenti Termini o ai Servizi sia sottoposto al tribunale federale o statale competente della Contea di San Francisco, California" (Dropbox)

REMEDY
------

-   Remedy\
    Definition: a clause establishing extra-contractual remedies such as injunction, penalties or other, in case of a violation of the contract. 

Category: remedy

Examples:\
"Dott si riserva il diritto di applicare una penale fino a 5 euro nel caso di parcheggio scorretto" (Dott)

Notes:

-   Any indications on the right to take part in a class action is INCLUDED, unless the clause pertains to an ADR provision:

Example:  "L'utente ed ea rinunciano espressamente al diritto di ricorrere a un processo tramite giuria e al diritto di partecipare a una class action" (EA)

TERMINATION
-----------

-   Termination_clause\
    Definition: a clause establishing whether a party can unilaterally terminate the contract, with or without stating their reasons.\
    Category: termination

Examples:

"L'Utente potrà cessare l'utilizzo del Software in qualsiasi momento" (Adobe)

Notes:

-   Any indications of contract's termination is INCLUDED even if the provision refers to the possibility of contract's renewal:\
    Example: "L'abbonamento si rinnova automaticamente finché l'utente non lo termina o annulla" (Tinder)

TERM
----

-   Termination_term\
    Definition: it refers to the temporal term of the termination clause.

Category: term

Examples:\
"immediatamente" in "Il presente Contratto si risolverà immediatamente al momento della cancellazione dell'account, salvo quanto previsto nella Sezione 25.4 sotto riportata" (Grindr)\
"In qualsiasi momento" in "Possiamo risolvere in qualsiasi momento il contratto stipulato con l'utente qualora" (Adobe)

-   Coverage_cap_term

Definition: the forewarning term to request the compensation connected to the violation of a contract provision. 

Category: term

Examples:\
"entro quattordici (14) giorni dal giorno in cui Grindr riceve la comunicazione relativa alla decisione di disdetta dei Servizi Premium da parte dell'Utente" (Grindr)

-   License_term\
    Definition: it refers to the temporal term of the license.

Category: term

Examples:

"il periodo di valutazione" in "L'utente può installare e utilizzare la Versione di valutazione solo durante il periodo di valutazione e solo a scopo di valutazione" (Adobe)

-   Renewal_term\
    Definition: it establishes the temporal term of contract's renewal (e.g., following number of days/months/years)\
    Category: term

Examples:\
"Grindr (direttamente o tramite un App Store) comunicherà all'Utente in anticipo la data di rinnovo dell'abbonamento dei Servizi Premium e dell'abbonamento di prova prima di effettuare l'addebito sulla carta di credito o di debito" (Grindr)

-   Forewarning_term\
    Definition: it refers to a forewarning term to comply with a contract provision (e.g., number of days/months/years).

Category: term

Notes:

-   The term referring to the termination or renewal of the contract is NOT INCLUDED:

Examples: "entro quattordici (14) giorni " in "L'Utente ha il diritto di recedere dai Servizi Premium di Grindr entro quattordici (14) giorni senza fornire alcuna motivazione" (Grindr)

IP
--

-   IP\
    Definition: allocation or management of rights related to the intellectual property of a product, service, or other item governed by the contract.

Domain: intellectual property

Examples:

"Noi (e i nostri licenziatari) rimaniamo gli esclusivi proprietari di qualsiasi diritto, titolo e interesse relativo al Software" (Adobe)

"Tutte le informazioni, i dati, i programmi informatici sottostanti (incluse le API), i nomi a dominio, gli URL, le banche dati, e i materiali presenti su questo sito web, ivi inclusi nomi, logo, programmi di volo, prezzi etc., nonché l'abbinamento di colori e il layout del sito web, sono tutelati dal diritto d'autore, diritti sui marchi registrati, diritti di privativa sulle banche dati e/o altri diritti di proprietà intellettuale" (Ryanair)

LICENSE
-------

-   License\
    Definition: the contract includes a license granted by one party to its counterpart, which is managed according to specific protocols. The license can impose restrictions on usage.\
    Domain: license

Examples:

"conferiamo all'utente la licenza non esclusiva per l'installazione e l'utilizzo del Software (a) nel territorio e (b) in conformità alle presenti condizioni e alla relativa documentazione che accompagna il Software" (Adobe)

Notes:

-   INCLUDED in the label are any descriptions or rules that better specify the use of the license:\
    Examples: "L'utente può installare e utilizzare la Versione di valutazione solo durante il periodo di valutazione e solo a scopo di valutazione" (Adobe)\
    "A meno che la documentazione o la licenza specifica correlata ai File di contenuto non indichi altrimenti, l'utente può utilizzare, visualizzare, modificare, riprodurre e distribuire tutti i File di contenuto" (Adobe)

-   INCLUDED in the label are any limitations in the use and sharing of the license:\
    Examples: "Se non consentito dalle presenti condizioni, l'utente non può...concedere in locazione, in leasing o in sublicenza, vendere, assegnare o trasferire i propri diritti sul Software oppure consentire la copia integrale o parziale del Software su dispositivi di terzi" (Adobe)

LIABILITY
---------

-   Liability_allocation\
    Definition: a party's liability for a breach of contractual obligations. It encompasses liability for specific types of breaches, such as breach of intellectual property or breach of confidentiality.

Domain: liability

Examples:

"L'utente accetta di risarcire Adobe per ogni e qualsiasi responsabilità, perdita, azione legale, danno o pretesa (compresi ragionevoli costi e spese legali) derivanti o connessi all'uso di o all'affidamento a qualsiasi certificato digitale o Autorità di certificazione" (Adobe)

-   Liability_exclusion\
    Definition: a party's liability for a breach of contractual obligations is excluded with regards to a specific case.

Domain: liability

Examples:

-   "Non siamo responsabili verso l'utente o terzi per danni speciali, incidentali, indiretti, consequenziali o punitivi di alcun tipo (anche qualora fossimo stati messi al corrente della possibilità del verificarsi di tali danni)" (Adobe)

-   Liability_limitation\
    Definition: a party's liability for a breach of contractual obligations is limited with regards to a specific case.\
    Domain:liability

Examples:

"saremo ritenuti responsabili solo per i danni diretti e immediati effettivamente subiti, pagati o a cui si è andati incontro, dovuti a una mancata osservanza dei nostri obblighi nel rispetto dei servizi che avremmo dovuto assolvere" (Booking)

WARRANTY
--------

-   Coverage_cap\
    Definition: it defines the scope of liability with regards to a contract breach. It may encompass the maximum amount that can be recovered.\
    Domain: warranty

    Examples:\
    "Nel rispetto dei presenti Termini e per quanto consentito dalla legge, la nostra massima responsabilità congiunta nei confronti dell'utente, derivante o in relazione a questi Termini o all'accesso a, uso di, o impossibilità ad accedere a o all'uso dei nostri Servizi o delle nostre Piattaforme è limitata alla somma di £100 (cento sterline britanniche)" (Skyscanner)

-   Warranty\
    Definition: it declares a form of guarantee against defects or errors in the technology, product or service provided under the contract.\
    Domain: warranty

Esempi: 

"Il Software viene fornito "COSÌ COME È"" (Adobe)

"decliniamo ogni garanzia, esplicita o implicita, incluse le garanzie implicite di non violazione, commerciabilità e idoneità per uno scopo particolare" (Adobe)

Notes:

-   INCLUDED in the label are any disclaimers:

Examples: "La Versione preliminare non rappresenta il prodotto finale e può contenere bug che possono causare guasti al sistema o di altro tipo e perdite di dati" (Adobe)

-   INCLUDED in the label are any content removal clauses:

Examples: "Ci riserviamo il diritto di esaminare la tua condotta e i tuoi contenuti affinché siano conformi ai presenti Termini e alle nostre Norme sull'uso accettabile" (Dropbox)

-   Insurance\
    Definition: a party declares to have provided insurance for the benefit of the other party or it may be explicitly stated that insurance is to be taken out for the benefit of the contract.\
    Domain: warranty

Examples: "Lo Studio ha una copertura assicurativa per la responsabilità professionale in forza di polizza stipulata dall'Associazione Professionale per Massimale di Euro 2.000.000"

-   Post_contract_obligation\
    Definition: a party is subject to obligations after termination or expiration of a contract, which can include post-termination commitments such as transition arrangements, payments, transfer of intellectual property, liquidation, last purchases, or similar obligations.\
    Domain: warranty

Examples:

"Dopo la scadenza o la risoluzione del presente contratto, eventuali licenze perpetue concesse, gli obblighi di indennizzo dell'utente, le nostre esclusioni di garanzia o limitazioni di responsabilità e le disposizioni per la composizione delle controversie ivi contenute resteranno validi" (Adobe)

ACCEPTANCE
----------

-   Contract_by_using\
    Definition: the clause determines implicit acceptance of the contract by the use of the service only.\
    Domain: acceptance

Examples:

"Utilizzando il Software, l'utente accetta dette condizioni" (Adobe)

-   Acceptance\
    Definition: it determines the manner of conclusion (i.e., acceptance of the proposal) of the contract.

Domain: acceptance

Examples:

"La conclusione del contratto avviene al momento dell'invio della Conferma d'Ordine da parte del Titolare all'indirizzo email fornito dall'Utente" (Gianvitorossi)

AMENDMENT
---------

-   Contract_amendment\
    Definition: the contract may be unilaterally amended by one party's will.\
    Domain: amendment

Examples:

"Potremmo modificare i presenti termini o eventuali termini aggiuntivi applicabili a un Servizio, ad esempio per rispecchiare modifiche apportate alle leggi o ai nostri Servizi" (Google)

-   Service_amendment\
    Definition: the clause allows either party to unilaterally change the means of contract execution (e.g. software upgrade).\
    Domain: amendment

Example:

"L'Utente accetta di ricevere tali aggiornamenti da Adobe come parte dell'uso del Software da parte dell'Utente" (Adobe)

Note:

-   INCLUDES unilateral amendments alternative to termination between the parties:

Example: "Anziché recedere dal presente Accordo e prima di un eventuale recesso, EA ha facoltà di avvisare l'utente, sospendere o modificare il suo accesso ad un particolare servizio EA o al suo Account EA, rimuovere o revocare diritti a livello di Account EA o di dispositivo, rimuovere o cancellare qualsiasi contenuto che violi il presente Accordo o impedire al dispositivo o alla macchina dell'utente di accedere a specifici servizi EA" (EA)

AUDIT
-----

-   Audit\
    Definition: it defines the means and procedures to verify the proper execution of the contract.

Domain: audit

Examples:

"Se l'utente rappresenta un'impresa, una società o un'organizzazione, possiamo, non più di una volta ogni 12 mesi e con preavviso di sette giorni, incaricare il nostro personale o un ispettore esterno indipendente, soggetto a obbligo di riservatezza, di controllare i registri, i sistemi e le strutture del cliente per verificare che l'installazione e l'uso di qualsiasi Software sia conforme alle valide licenze d'uso da noi rilasciate" (Adobe)

DATA PROTECTION
---------------

-   Data_protection\
    Definition: it defines the use, rights and obligations related to the processing of personal data of the parties and third parties in connection to the contract.

Domain: data protection

Examples:

"Grindr conserverà i registri delle applicazioni in virtù della riservatezza, in un ambiente controllato e sicuro, per sei (6) mesi dalla data di sottoscrizione" (Grindr)

Notes:

-   References to privacy policies and other data protection documents are INCLUDED:

Example: to "Consultare la nostra Informativa sulla privacy per ulteriori informazioni relative a uso, raccolta o condivisione delle informazioni, compresi i Contenuti dell'utente" (Grindr)
