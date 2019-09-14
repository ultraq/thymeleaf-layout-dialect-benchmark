
Thymeleaf Layout Dialect benchmarking web app
=============================================

A basic web application to test the memory profile of the
[Thymeleaf Layout Dialect](https://github.com/ultraq/thymeleaf-layout-dialect).

Testing currently requires some manual coordination of the web application
(`./gradlew bootRun`) and the JMeter test (`./gradlew jmeter`).  Either the IDE
can run both in parallel, or use multiple shell sessions to run both in parallel.

Once run, JMeter's HTML reports can be found in `build/reports/(dialect-version)/(date-time-of-run)`.

To include YourKit profiling for memory snapshots, then the agent needs to be
loaded with the web application via the `-agentpath` VM argument.  eg: on MacOS:

`-agentpath:"/Applications/YourKit Java Profiler 2015.app/Contents/Resources/bin/mac/libyjpagent.jnilib"`
