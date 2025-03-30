# observability-playground


## Attach to any JVM-Process
To attach an apm-agent after starting a jvm-app first
get the apm-agent (see [Automatic setup with apm-agent-attach-cli.jar](https://www.elastic.co/guide/en/apm/agent/java/current/setup-attach-cli.html))

then run for example 
```
java -jar .\apm-agent-attach-cli-1.52.2.jar --include-main org.springframework.samples.petclinic.PetClinicApplication spring-petclinic-3.4.0-SNAPSHOT.jar
```
this uses the `elasticapm.properties`. 

## Setup with Java-Agent

Another option is to run the Agent with the Application. See [Elastic-Documentation: Manual setup with -javaagent flag](https://www.elastic.co/guide/en/apm/agent/java/current/setup-javaagent.html)

## Programmatic Setup

See [Elastic-Documentation: Programmatic API setup to self-attach
](https://www.elastic.co/guide/en/apm/agent/java/current/setup-attach-api.html)