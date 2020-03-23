---


---

<h1 id="sqlite-windows版本安装指南"><strong>SQLite Windows版本安装指南</strong></h1>
<p><strong>关于SQLite</strong><br>
SQLite是一款SQL数据库引擎，无需额外服务器即可进行关系数据库管理。这款轻量化的数据库无需任何配置，可直接对原硬盘文档进行读写。</p>
<h2 id="下载sqlite">下载SQLite</h2>
<p>若需SQLite, 打开SQLite官网<a href="https://www.sqlite.org/download.html">下载页面</a>。</p>
<ol>
<li>前往 <a href="https://www.sqlite.org/download.html">https://www.sqlite.org/download.html</a></li>
<li>选择一款适配您的操作系统的SQLite版本。对于您Windows操作系统，请下拉页面至 <code>Precompiled Binaries for Windows</code>。<br>
<img src="https://cdn.sqlitetutorial.net/wp-content/uploads/2019/08/SQLite3-Windows-Download.png" alt="SQLite download page"></li>
<li>下载适配您的Windows系统版本的SQLite。</li>
</ol>
<h2 id="运行sqlite">运行SQLite</h2>
<p>SQLite是一款零配置数据库，文档以ZIP压缩形式供下载。 若需运行SQLite，请参考以下步骤：</p>
<ol>
<li>将压缩文档解压至您的本地硬盘 (C:) ，并创建一个新文件夹，如 <code>C:\sqlite</code><br>
<img src="https://cdn.sqlitetutorial.net/wp-content/uploads/2019/08/SQLite3-tools.png" alt="ZIP file contents"></li>
<li>运行<strong>命令提示符</strong>程序</li>
<li>使用<strong>改变目录</strong> 命令以导航至您创建的文件夹：</li>
</ol>
<pre><code>  1. C:\&gt;cd C:\&gt;sqlite
  2. C:\&gt;sqlite&gt;
</code></pre>
<ol start="4">
<li>输入 <code>sqlite3</code>并按回车键，即可进入SQL数据库。您将看到下列文字输出：</li>
</ol>
<pre><code>SQLite version 3.31.1 2020-01-27 19:55:54
Enter ".help" for usage hints.
Connected to a transient in-memory database.
Use ".open FILENAME" to reopen on a persistent database.
</code></pre>
<ol start="5">
<li>您可以通过输入 <code>.help</code> 指令，获取SQLite数据库详细指令列表。</li>
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
<li>若需退出SQLite，输入<code>.quit</code>并按回车键.</li>
</ol>

