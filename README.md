# sscce_jdkfxproblem
SSCCE of problem building JavaFX 11 app with a JDK 13 including JavaFX

With `<release>11</release>` the following command renders BUILD SUCCESS
`JAVA_HOME=/atlas/data-config/.sdkman/candidates/java/11.0.7.fx-zulu/ mvn clean install`

Using 
`JAVA_HOME=/atlas/data-config/.sdkman/candidates/java/13.0.3.fx-zulu/ mvn clean install` does not.

COMPILATION ERROR : 
package javafx.util does not exist

Removing `<release>11</release>` or replacing it with source and target makes it work again.

Is it possible to use the latest (bundled) JavaFX while targeting Java 11?
