<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>DB</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__left">
    <div class="stackedit__toc">
      
<ul>
<li><a href="#soluzioni-azure-per-db">Soluzioni Azure per DB</a></li>
<li><a href="#azure-compute-services">Azure Compute Services</a></li>
</ul>

    </div>
  </div>
  <div class="stackedit__right">
    <div class="stackedit__html">
      <h1 id="soluzioni-azure-per-db">Soluzioni Azure per DB</h1>
<p>🪐<strong>Azure Cosmos DB:</strong> un servizio di database multimodale distribuito che è in grado di scalare per throughput e regioni. E’ accessibile attraverso delle API.<br>
Supporta dati schemaless e, a basso livello, i dati sono salvati in formato Atom-Record-Sequence (ARS):</p>
<ul>
<li><em>atomi</em>, primitive (string, bool…)</li>
<li><em>record</em>, struct</li>
<li><em>sequenze</em>, array di atomi, record o sequenze</li>
</ul>
<p>I dati sono astratti e proiettati via API da specificare all’atto della creazione del db (SQL, MongoDB, Cassandra, Tables, Gremlin)</p>
<p>📑<strong>Azure SQL Database:</strong> è un db relazionale basato sull’ultima versione community di SQL Server. E’ un database PaaS, che garantisce il 99.99% di availability. E’ totalmente managed e può gestire sia dati relazionali che non relazionali (json, xml, dati spaziali…)<br>
La migrazione verso questo database è assistita tramite <em>Azure Database Migration Service</em>, che crea un report per la migrazione.</p>
<p>🔧<strong>Azure SQL Managed Instance:</strong> offre alcune funzionalità in più rispetto ad Azure SQL Database (per es. si possono usare collation non latine).</p>
<p>🐬<strong>Azure Database for MySQL:</strong> è un servizio di database basato sulla versione community di MySQL (v. 5.6, 5.7, 8.0)</p>
<p>🐘<strong>Azure Database for PostgreSQL:</strong> è un servizio basato sulla versione community di PostgreSQL.<br>
E’ disponibile in due versioni:</p>
<ul>
<li><em>Single server</em>: scala verticalmente</li>
<li><em>Hyperscale</em> (citus): scala con sharding. E’ generalmente usato per carichi che eccedano i 100GB di dati.</li>
</ul>
<h1 id="azure-compute-services">Azure Compute Services</h1>
<p>Azure Compute Services raccoglie una serie di servizi on-demand per far girare applicazioni sul Cloud.</p>
<p><strong>Azure Virtual Machines</strong> (IaaS): macchine virtuali che è possibile customizzare totalmente. Configurazione, update e manutenzione sono a carico dell’utente.<br>
E’ possibile creare VM a partire da template.<br>
E’ possibile migrare ambienti ed applicazioni da un server fisico ad una VM in Cloud (lift and shift).</p>
<p>Virtual machine scale sets permettono di fare deploy di VM identiche e di gestirle per beneficiare del load balancing. Il numero di VM coinvolte scala automaticamente in base alla richiesta.</p>
<p>Azure Batch: esegue job batch scalandoli su moltissime VM.</p>
<p><strong>Containers e Kubernetes</strong>: sono finalizzati al deploy e al management di containers.</p>
<p><strong>App Service</strong>:  permette di fare build, deploy e scale di applicazioni web, mobile e API per ogni tipo di piattaforma.</p>
<p><strong>Functions</strong>: utilizzate per lanciare codice in corrispondenza del verificarsi di alcuni eventi o alla ricezione di messaggi da altri servizi Azure.</p>

    </div>
  </div>
</body>

</html>
