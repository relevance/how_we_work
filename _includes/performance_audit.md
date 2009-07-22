### Performance Audit {#performance_audit}

A typical performance audit for a web application will include:

* Baseline Reporting: For Rails applications we use RPM, by [New Relic](http://www.newrelic.com), to establish a baseline understanding of the performance characteristics of your application.
* Database Analysis: We look at your database infrastructure, from installed versions of the database engine to schema decisions and everything in between.
* External Process Analysis: Are you using Solr for searching? What about ActiveMQ as a messaging infrastructure? We'll look at how your processes are managed, and the communication channels between them and your Rails application, to find drags and bottlenecks.
* Server Analysis: We study your server environment to ensure that the right tools are enabled, the wrong ones removed, and that your host is providing the right environment for your application to run in.

We generally fix a number of bottlenecks during the Audit. At the end of the Audit we produce a detailed report of these fixes, plus any areas of concern that you need to fix.