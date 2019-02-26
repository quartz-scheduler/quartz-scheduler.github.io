
<div class="secNavPanel"><a href=".">Contents</a> | <a href="CreateScheduler.md">&lsaquo;&nbsp;Prev</a> | <a href="ShutdownScheduler.md">Next&nbsp;&rsaquo;</a></div>





# How-To: Placing a Scheduler in Stand-by Mode

### Placing a Scheduler in Stand-by Mode

<pre class="prettyprint highlight"><code class="language-java" data-lang="java">
// start() was previously invoked on the scheduler

scheduler.standby();

// now the scheduler will not fire triggers / execute jobs

// ...

scheduler.start();

// now the scheduler will fire triggers and execute jobs
</code></pre>
