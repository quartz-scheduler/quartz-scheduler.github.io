
<div class="secNavPanel"><a href=".">Contents</a> | <a href="ListTriggers.md">&lsaquo;&nbsp;Prev</a> | <a href="JobListeners.md">Next&nbsp;&rsaquo;</a></div>





# How-To: Finding Triggers of a Job


### Finding Triggers of a Job

<pre class="prettyprint highlight"><code class="language-java" data-lang="java">
List&lt;Trigger&gt; jobTriggers = sched.getTriggersOfJob(jobKey("jobName", "jobGroup"));
</code></pre>
