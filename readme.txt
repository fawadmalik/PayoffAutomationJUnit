1. Install Java SDK 1.7 from oracle
2. Install Maven 3.2.5 from Apache
3. Edit .bash_profile by adding the following:

export JAVA_HOME=$(/usr/libexec/java_home)
export M2_HOME=/Users/myang/apache-maven-3.2.5
export PATH=$PATH:$M2_HOME/bin

4. Unzip PayoffAutomationJUnit
5. Go to PayoffAutomationJUnit folder via command line and type the following:
> mvn clean install

or

> mvn clean test -Dgroups="com.payoff.SetupTests" -X

or

> mvn clean test -Dgroups=SetupTests -X

6. WebDriver will kick to execute few tests
