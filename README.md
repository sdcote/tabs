# Tabs

This is a project which started years ago in the Telecommunication industry in response to the problem of monitoring and managing hundreds of critical applications and their subsystems. Back then monitoring and management (M&M) was a concept applied mainly to hardware infrastructure; DMX, servers, switches, routers, SAN and the like. As more projects adopted agile methodologies and decisions increasingly relying on empirical data, it became clear that logical systems needed to generate metrics and events to help teams received immediate feedback. Instrumenting systems in the same manner as devices seems the most logical next step. A team of IT agilists started project Argus (after Argus Panoptes) to create a library enabling the monitoring and management of IT developed applications. Over the years, the instrumented applications allowed their developers to monitor and manage all aspects of the applications, allowing the teams to greatly enhance the quality of their software, its reliability, availability, and reduce overall operations and maintenance costs.

Tabs models that same approach albeit with modern goals. Now in the age of 12-factor applications, micro services, containerization, and the rise of componentized architecture implementations, teams are looking for a simple, low-cost, M&M solution which does not tie their approach to any one technology, platform, or product. Tabs is that project.

Adding a JAR to your Java project allows you to collect events and metrics which can be sent to any number of M&M platforms. Tabs is an instrumentation (i13n) library. It provides very simple fixtures your logic can use to track timings, evets, counters, states and gauges. These "sensors" are called by your code to collect data and export it. That's it.

Tab calls are designed to be left in your code in all environments. Actual metric collection and processing only occur when enabled, meaning you only incur the cost of data collection when it is necessary.  Current tests have shown leaving these calls in the code only incur a 0.3 microsecond tax on performance but enable the development team to "switch on" metric collection when problems are being diagnosed without bringing down the component or otherwise loosing data in memory. This means development teams can diagnose problems as they occur with the data in memory which are causing those problems. This real-time monitoring has proven invaluable in solving production problems and opens the door to managing application component instances.

### Why the name "Tabs"?
This is a library which will allow you to keep tabs on all your components.

## Future Plans

The original Argos project included both JAR and a DLL version. Future versions of Tabs will contain a DLL version for Mono and .NET components.
