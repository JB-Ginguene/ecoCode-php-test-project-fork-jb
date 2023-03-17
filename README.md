Purpose of this project
---

To check locally all rules on PHP language.
To do this :

- first launch local development environment (SonarQube)
- launch sonar maven command to send sonar metrics to local SonarQube
- on local SonarQube, check if each PHP file contains (or not) the rule error defined for this class

Step 1 : prepare local environment
---

To launch local environment : please follow https://github.com/green-code-initiative/ecoCode/blob/main/INSTALL.md
(especially SonarQube configuration part)

Step 2 : send Sonar metrics to local SonarQube
---

`mvn org.sonarsource.scanner.maven:sonar-maven-plugin:3.9.1.2184:sonar -Dsonar.login=MY_SONAR_TOKEN`

Step 3 : check errors
---

on local SonarQube, check if each PHP file contains (or not) the rule error defined for this class
(for example : you can search for tag `eco-design` rule on a special file)
