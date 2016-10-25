
Thymeleaf Layout Dialect benchmarking web app
=============================================

A basic web application to test the memory profile of the
[Thymeleaf Layout Dialect](https://github.com/ultraq/thymeleaf-layout-dialect).

Testing is currently done by running this web app with a max heap size of 512MB
(`-Xmx512m`), and run with the YourKit profiler agent.  The client program is
then attached and additional monitoring of object allocations is added.  Then,
JMeter is brought into the mix, running the load simulation plan in the `JMeter`
directory.
