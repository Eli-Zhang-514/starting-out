---


---

<h1 id="sqlite-installation-guide-for-windows"><strong>SQLite Installation Guide for Windows</strong></h1>
<p><strong>About SQLite</strong><br>
SQLite is a SQL database engine which provides relational database management without an additional server progress. The light-weight software library requires zero configuration as it reads and writes directly to original disk files.</p>
<h2 id="download-sqlite">Download SQLite</h2>
<p>To download SQLite, open the <a href="https://www.sqlite.org/download.html">download page</a> of the SQlite official website.</p>
<ol>
<li>Go to <a href="https://www.sqlite.org/download.html">https://www.sqlite.org/download.html</a></li>
<li>Choose an SQLite precompiled binaries for your OS. In this case, scroll down to <code>Precompiled Binaries for Windows</code><br>
<img src="https://cdn.sqlitetutorial.net/wp-content/uploads/2019/08/SQLite3-Windows-Download.png" alt="SQLite download page"></li>
<li>Download the appropriote version for your Windows system.</li>
</ol>
<h2 id="run-sqlite">Run SQLite</h2>
<p>As SQLite is a zero-configuration library, the downloaded file comes in the ZIP format. To run SQLite tools, follow the steps below:</p>
<ol>
<li>Extrat the contents of the ZIP file to your local drive (C:) in a folder, e.g. <code>C:\sqlite</code><br>
<img src="https://cdn.sqlitetutorial.net/wp-content/uploads/2019/08/SQLite3-tools.png" alt="ZIP file contents"></li>
<li>Run the <strong>Command Prompt</strong> program</li>
<li>Navigate to the folder you created using the <strong>Change Directory</strong> command:</li>
</ol>
<pre><code>  1. C:\&gt;cd C:\&gt;sqlite
  2. C:\&gt;sqlite&gt;
</code></pre>
<ol start="4">
<li>Enter the SQLite library by inputting <code>Sqlite3</code>and press Enter. You will see the following output:</li>
</ol>
<pre><code>SQLite version 3.31.1 2020-01-27 19:55:54
Enter ".help" for usage hints.
Connected to a transient in-memory database.
Use ".open FILENAME" to reopen on a persistent database.
</code></pre>
<ol start="5">
<li>You can input <code>.help</code> for a detailed list of commands within the SQLite library</li>
</ol>
<pre><code>sqlite&gt; .help
.archive ...             Manage SQL archives
.auth ON|OFF             Show authorizer callbacks
.backup ?DB? FILE        Backup DB (default "main") to FILE
.bail on|off             Stop after hitting an error.  Default OFF
.binary on|off           Turn binary output on or off.  Default OFF
.cd DIRECTORY            Change the working directory to DIRECTORY
.changes on|off          Show number of rows changed by SQL
.check GLOB              Fail if output since .testcase does not match
.clone NEWDB             Clone data into NEWDB from the existing database
.databases               List names and files of attached databases
.dbconfig ?op? ?val?     List or change sqlite3_db_config() options
.dbinfo ?DB?             Show status information about the database
.dump ?TABLE? ...        Render all database content as SQL
.echo on|off             Turn command echo on or off
.eqp on|off|full|...     Enable or disable automatic EXPLAIN QUERY PLAN
.excel                   Display the output of next command in spreadsheet
.exit ?CODE?             Exit this program with return-code CODE
.expert                  EXPERIMENTAL. Suggest indexes for queries
.explain ?on|off|auto?   Change the EXPLAIN formatting mode.  Default: auto
.filectrl CMD ...        Run various sqlite3_file_control() operations
.fullschema ?--indent?   Show schema and the content of sqlite_stat tables
.headers on|off          Turn display of headers on or off
.help ?-all? ?PATTERN?   Show help text for PATTERN
.import FILE TABLE       Import data from FILE into TABLE
.imposter INDEX TABLE    Create imposter table TABLE on index INDEX
.indexes ?TABLE?         Show names of indexes
.limit ?LIMIT? ?VAL?     Display or change the value of an SQLITE_LIMIT
.lint OPTIONS            Report potential schema issues.
.load FILE ?ENTRY?       Load an extension library
.log FILE|off            Turn logging on or off.  FILE can be stderr/stdout
.mode MODE ?TABLE?       Set output mode
.nullvalue STRING        Use STRING in place of NULL values
.once (-e|-x|FILE)       Output for the next SQL command only to FILE
.open ?OPTIONS? ?FILE?   Close existing database and reopen FILE
.output ?FILE?           Send output to FILE or stdout if FILE is omitted
.parameter CMD ...       Manage SQL parameter bindings
.print STRING...         Print literal STRING
.progress N              Invoke progress handler after every N opcodes
.prompt MAIN CONTINUE    Replace the standard prompts
.quit                    Exit this program
.read FILE               Read input from FILE
.recover                 Recover as much data as possible from corrupt db.
.restore ?DB? FILE       Restore content of DB (default "main") from FILE
.save FILE               Write in-memory database into FILE
.scanstats on|off        Turn sqlite3_stmt_scanstatus() metrics on or off
.schema ?PATTERN?        Show the CREATE statements matching PATTERN
.selftest ?OPTIONS?      Run tests defined in the SELFTEST table
.separator COL ?ROW?     Change the column and row separators
.sha3sum ...             Compute a SHA3 hash of database content
.shell CMD ARGS...       Run CMD ARGS... in a system shell
.show                    Show the current values for various settings
.stats ?on|off?          Show stats or turn stats on or off
.system CMD ARGS...      Run CMD ARGS... in a system shell
.tables ?TABLE?          List names of tables matching LIKE pattern TABLE
.testcase NAME           Begin redirecting output to 'testcase-out.txt'
.testctrl CMD ...        Run various sqlite3_test_control() operations
.timeout MS              Try opening locked tables for MS milliseconds
.timer on|off            Turn SQL timer on or off
.trace ?OPTIONS?         Output each SQL statement as it is run
.vfsinfo ?AUX?           Information about the top-level VFS
.vfslist                 List all available VFSes
.vfsname ?AUX?           Print the name of the VFS stack
.width NUM1 NUM2 ...     Set column widths for "column" mode
sqlite&gt; .quit
</code></pre>
<ol start="6">
<li>To quit SQLite, input <code>.quit</code> and press Enter.</li>
</ol>

