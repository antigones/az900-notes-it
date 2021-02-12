---


---

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

