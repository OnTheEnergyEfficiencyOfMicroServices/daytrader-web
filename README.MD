# DayTrader Web

The Web UI from the daytrader application.

## Prerequisites

### Java 8
```
sudo apt install openjdk-8-jdk
```
```
sudo update-alternatives --config java
```
```
sudo update-alternatives --config javac
```
```
java -version
```
[Linux Guide](https://linuxconfig.org/how-to-install-and-switch-java-versions-on-ubuntu-linux)

### Maven 3.3.9+
```
sudo apt install maven
```
```
mvn -v
```

## Build, Release, and Run


### Build

1.  `$ cd daytrader-webapp`

2.  `$ mvn package`

    This command builds the Spring Boot executable WAR

### Start

1.  `$ cd daytrader-web`

2.  `$ ./env/external/springboot/bin/start_server.sh`

    This command runs the Spring Boot executable WAR

https://localhost:5443/

### Review the Swagger Documentation

1.  https://localhost:5443/swagger-ui.html

<hr>

### Test the Web UI

1.  Start the Accounts, Gateway, Portfolios, and Quotes

2.  Open your browser and navigate to: `https://localhost:5443`

3.  Under the Configuration Tab

    a.  Press(Re)-create DayTrader Database Tables and Indexes
    
    b.  Press (Re)-populate DayTrader Database

    c.  Press Test Daytrader Scenario

4.  Keep refreshing the browser until you are satisfied that DayTrader is working. 

    Note that each time you refresh the browser, it runs a random functional test. 
   
    That's it! You have now tested the DayTader
    
5.  Stop the Accounts, Gateway, Portfolios, and Quotes
