
<div class="secNavPanel"><a href=".">Contents</a> | <a href="JobInitPlugin.md">&lsaquo;&nbsp;Prev</a> | <a href="ListTriggers.md">Next&nbsp;&rsaquo;</a></div>





# How-To: Listing Jobs in the Scheduler

### Listing all Jobs in the scheduler

<pre class="prettyprint highlight"><code class="language-java" data-lang="java">
// enumerate each job group
for(String group: sched.getJobGroupNames()) {
    // enumerate each job in group
    for(JobKey jobKey : sched.getJobKeys(groupEquals(group))) {
        System.out.println("Found job identified by: " + jobKey);
    }
}
</code></pre>
