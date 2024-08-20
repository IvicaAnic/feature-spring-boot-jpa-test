# Spring Boot + Spring Data JPA example

This is the source code for [Spring Boot + Spring Data JPA example](https://mkyong.com/spring-boot/spring-boot-spring-data-jpa/)

## Technologies used:
* Spring Boot 3.1.2
* Spring Data JPA (Hibernate 6  is the default JPA implementation)
* H2 in-memory database
* Maven
* Java 17
* JUnit 5

## How to run it
```
$ git clone https://github.com/IvicaAnic/feature-spring-boot-jpa-test

$ cd spring-data-jpa

$ ./mvnw spring-boot:run

INFO  com.ivica.anic.MainApplication - Starting MainApplication using Java 17.0.12 with PID 8960 (D:\angular\spring-boot-master\spring-data-jpa\target\classes started by Hp in D:\angular\spring-boot-master\spring-data-jpa)
INFO  com.ivica.anic.MainApplication - No active profile set, falling back to 1 default profile: "default"
INFO  o.s.d.r.c.RepositoryConfigurationDelegate - Bootstrapping Spring Data JPA repositories in DEFAULT mode.
INFO  o.s.d.r.c.RepositoryConfigurationDelegate - Finished Spring Data repository scanning in 57 ms. Found 1 JPA repository interfaces.
DEBUG com.zaxxer.hikari.HikariConfig - Driver class org.h2.Driver found in Thread context class loader jdk.internal.loader.ClassLoaders$AppClassLoader@2a139a55
DEBUG com.zaxxer.hikari.HikariConfig - HikariPoolZZZ - configuration:
DEBUG com.zaxxer.hikari.HikariConfig - allowPoolSuspension.............false
DEBUG com.zaxxer.hikari.HikariConfig - autoCommit......................true
DEBUG com.zaxxer.hikari.HikariConfig - catalog.........................none
DEBUG com.zaxxer.hikari.HikariConfig - connectionInitSql...............none
DEBUG com.zaxxer.hikari.HikariConfig - connectionTestQuery.............none
DEBUG com.zaxxer.hikari.HikariConfig - connectionTimeout...............20000
DEBUG com.zaxxer.hikari.HikariConfig - dataSource......................none
DEBUG com.zaxxer.hikari.HikariConfig - dataSourceClassName.............none
DEBUG com.zaxxer.hikari.HikariConfig - dataSourceJNDI..................none
DEBUG com.zaxxer.hikari.HikariConfig - dataSourceProperties............{password=<masked>}
DEBUG com.zaxxer.hikari.HikariConfig - driverClassName................."org.h2.Driver"
DEBUG com.zaxxer.hikari.HikariConfig - exceptionOverrideClassName......none
DEBUG com.zaxxer.hikari.HikariConfig - healthCheckProperties...........{}
DEBUG com.zaxxer.hikari.HikariConfig - healthCheckRegistry.............none
DEBUG com.zaxxer.hikari.HikariConfig - idleTimeout.....................600000
DEBUG com.zaxxer.hikari.HikariConfig - initializationFailTimeout.......1
DEBUG com.zaxxer.hikari.HikariConfig - isolateInternalQueries..........false
DEBUG com.zaxxer.hikari.HikariConfig - jdbcUrl.........................jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05;DB_CLOSE_DELAY=-1;DB_CLOSE_ON_EXIT=FALSE
DEBUG com.zaxxer.hikari.HikariConfig - keepaliveTime...................0
DEBUG com.zaxxer.hikari.HikariConfig - leakDetectionThreshold..........0
DEBUG com.zaxxer.hikari.HikariConfig - maxLifetime.....................1800000
DEBUG com.zaxxer.hikari.HikariConfig - maximumPoolSize.................5
DEBUG com.zaxxer.hikari.HikariConfig - metricRegistry..................none
DEBUG com.zaxxer.hikari.HikariConfig - metricsTrackerFactory...........none
DEBUG com.zaxxer.hikari.HikariConfig - minimumIdle.....................5
DEBUG com.zaxxer.hikari.HikariConfig - password........................<masked>
DEBUG com.zaxxer.hikari.HikariConfig - poolName........................"HikariPoolZZZ"
DEBUG com.zaxxer.hikari.HikariConfig - readOnly........................false
DEBUG com.zaxxer.hikari.HikariConfig - registerMbeans..................false
DEBUG com.zaxxer.hikari.HikariConfig - scheduledExecutor...............none
DEBUG com.zaxxer.hikari.HikariConfig - schema..........................none
DEBUG com.zaxxer.hikari.HikariConfig - threadFactory...................internal
DEBUG com.zaxxer.hikari.HikariConfig - transactionIsolation............default
DEBUG com.zaxxer.hikari.HikariConfig - username........................"sa"
DEBUG com.zaxxer.hikari.HikariConfig - validationTimeout...............5000
INFO  com.zaxxer.hikari.HikariDataSource - HikariPoolZZZ - Starting...
INFO  com.zaxxer.hikari.pool.HikariPool - HikariPoolZZZ - Added connection conn0: url=jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05 user=SA
INFO  com.zaxxer.hikari.HikariDataSource - HikariPoolZZZ - Start completed.
DEBUG com.zaxxer.hikari.pool.HikariPool - HikariPoolZZZ - Pool stats (total=1, active=0, idle=1, waiting=0)
DEBUG com.zaxxer.hikari.pool.HikariPool - HikariPoolZZZ - Added connection conn1: url=jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05 user=SA
DEBUG com.zaxxer.hikari.pool.HikariPool - HikariPoolZZZ - Added connection conn2: url=jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05 user=SA
DEBUG com.zaxxer.hikari.pool.HikariPool - HikariPoolZZZ - Added connection conn3: url=jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05 user=SA
DEBUG com.zaxxer.hikari.pool.HikariPool - HikariPoolZZZ - Added connection conn4: url=jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05 user=SA
DEBUG com.zaxxer.hikari.pool.HikariPool - HikariPoolZZZ - After adding stats (total=5, active=0, idle=5, waiting=0)
INFO  o.s.o.j.p.SpringPersistenceUnitInfo - No LoadTimeWeaver setup: ignoring JPA class transformer
INFO  o.s.o.j.LocalContainerEntityManagerFactoryBean - Initialized JPA EntityManagerFactory for persistence unit 'default'
INFO  o.s.d.j.r.query.QueryEnhancerFactory - Hibernate is in classpath; If applicable, HQL parser will be used.
INFO  com.ivica.anic.MainApplication - Started MainApplication in 3.111 seconds (process running for 3.453)
INFO  com.ivica.anic.MainApplication - findAll(), expect 4 books
INFO  com.ivica.anic.MainApplication - -------------------------------
INFO  com.ivica.anic.MainApplication - Book{id=1, title='Book A', price=9.99, publishDate=2023-08-31}
INFO  com.ivica.anic.MainApplication - Book{id=2, title='Book B', price=19.99, publishDate=2023-07-31}
INFO  com.ivica.anic.MainApplication - Book{id=3, title='Book C', price=29.99, publishDate=2023-06-10}
INFO  com.ivica.anic.MainApplication - Book{id=4, title='Book D', price=39.99, publishDate=2023-05-05}
INFO  com.ivica.anic.MainApplication -

INFO  com.ivica.anic.MainApplication - Book found with findById(1L):
INFO  com.ivica.anic.MainApplication - --------------------------------
INFO  com.ivica.anic.MainApplication - Book{id=1, title='Book A', price=9.99, publishDate=2023-08-31}
INFO  com.ivica.anic.MainApplication -

INFO  com.ivica.anic.MainApplication - Book found with findByTitle('Book B')
INFO  com.ivica.anic.MainApplication - --------------------------------------------
INFO  com.ivica.anic.MainApplication - Book{id=3, title='Book C', price=29.99, publishDate=2023-06-10}
INFO  com.ivica.anic.MainApplication -

INFO  com.ivica.anic.MainApplication - Book found with findByPublishedDateAfter(), after 2023/7/1
INFO  com.ivica.anic.MainApplication - --------------------------------------------
INFO  com.ivica.anic.MainApplication - Book{id=1, title='Book A', price=9.99, publishDate=2023-08-31}
INFO  com.ivica.anic.MainApplication -

INFO  com.ivica.anic.MainApplication - Book{id=2, title='Book B', price=19.99, publishDate=2023-07-31}
INFO  com.ivica.anic.MainApplication -

INFO  com.ivica.anic.MainApplication - Book delete where ID = 2L
INFO  com.ivica.anic.MainApplication - --------------------------------------------
INFO  com.ivica.anic.MainApplication - findAll() again, expect 3 books
INFO  com.ivica.anic.MainApplication - -------------------------------
INFO  com.ivica.anic.MainApplication - Book{id=1, title='Book A', price=9.99, publishDate=2023-08-31}
INFO  com.ivica.anic.MainApplication - Book{id=3, title='Book C', price=29.99, publishDate=2023-06-10}
INFO  com.ivica.anic.MainApplication - Book{id=4, title='Book D', price=39.99, publishDate=2023-05-05}
INFO  com.ivica.anic.MainApplication -

INFO  o.s.o.j.LocalContainerEntityManagerFactoryBean - Closing JPA EntityManagerFactory for persistence unit 'default'
INFO  com.zaxxer.hikari.HikariDataSource - HikariPoolZZZ - Shutdown initiated...
DEBUG com.zaxxer.hikari.pool.HikariPool - HikariPoolZZZ - Before shutdown stats (total=5, active=0, idle=5, waiting=0)
DEBUG com.zaxxer.hikari.pool.PoolBase - HikariPoolZZZ - Closing connection conn0: url=jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05 user=SA: (connection evicted)
DEBUG com.zaxxer.hikari.pool.PoolBase - HikariPoolZZZ - Closing connection conn1: url=jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05 user=SA: (connection evicted)
DEBUG com.zaxxer.hikari.pool.PoolBase - HikariPoolZZZ - Closing connection conn2: url=jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05 user=SA: (connection evicted)
DEBUG com.zaxxer.hikari.pool.PoolBase - HikariPoolZZZ - Closing connection conn3: url=jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05 user=SA: (connection evicted)
DEBUG com.zaxxer.hikari.pool.PoolBase - HikariPoolZZZ - Closing connection conn4: url=jdbc:h2:mem:6c28c77a-0ade-4bd2-9038-3be9aa3a1b05 user=SA: (connection evicted)
DEBUG com.zaxxer.hikari.pool.HikariPool - HikariPoolZZZ - After shutdown stats (total=0, active=0, idle=0, waiting=0)
INFO  com.zaxxer.hikari.HikariDataSource - HikariPoolZZZ - Shutdown completed.
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  5.438 s
[INFO] Finished at: 2024-08-20T02:50:54+02:00
[INFO] ------------------------------------------------------------------------
PS D:\angular\spring-boot-master\spring-data-jpa>




```


