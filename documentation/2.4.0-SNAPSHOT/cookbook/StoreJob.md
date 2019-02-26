
<div class="secNavPanel"><a href=".">Contents</a> | <a href="UnscheduleJob.md">&lsaquo;&nbsp;Prev</a> | <a href="ScheduleStoredJob.md">Next&nbsp;&rsaquo;</a></div>





# How-To: Storing a Job for Later Use

### Storing a Job

<pre class="prettyprint highlight"><code class="language-java" data-lang="java">
// Define a durable job instance (durable jobs can exist without triggers)
JobDetail job1 = newJob(MyJobClass.class)
    .withIdentity("job1", "group1")
    .storeDurably()
    .build();

// Add the the job to the scheduler's store
sched.addJob(job, false);
</code></pre>
