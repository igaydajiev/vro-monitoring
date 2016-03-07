Enables Hibernate Statistics JMX bean for vRealize Orchestrator 5.5.x

How to use it :
1. Copy the vro-database-statistics.jar file into '{vRO Instalation}/app-server/deploy/vco/WEB-INF/lib' folder
2. Restart vRO Server
3. Open jconsole and connect to vRO server JMX 
4. Locate Hibernate->Statistics bean
5. To enable gathering of statistic invoke setStatisticsEnabled(true) method

For visualization of statistics data hibernate-jconsole plugin can be used. hibernate-jconsole plugin can be downloaded from (http://hibernate-jcons.sourceforge.net/)
This plugin can be used for for visualizing the statistics info.
For details see http://hibernate-jcons.sourceforge.net/usage.html


java -Dhibernate.classpath={PATH_TO_FOLDER_HIBERNATE_JARS}/app-server/deploy/vco/WEB-INF/lib;./; -jar hibernate-jconsole-1.0.7.jar