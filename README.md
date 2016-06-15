# crypto-encrypt-util
custom util to get encrypted password for WSO2

### How to build and run
run `mvn clean install`

Note - below step is redundant now
create a directory call *lib* and copy the build jar (crypto-encrypt-util-1.0-SNAPSHOT.jar) to the lib directory.
copy the following jars to the lib directory (from .m2)
* axiom-api-1.2.11.jar
* bcprov-jdk16-1.46.jar

run the *encrypt* script as follows

`./encrypt <plainTextPassword> <keystoreFilePath> <keystoreFilePassword> <certificateAlias>`


### Useful Commands

* mkdir lib;
* cp target/crypto-encrypt-util-1.0-SNAPSHOT.jar lib/.;
* cp ~/.m2/repository/org/apache/ws/commons/axiom/axiom-api/1.2.11/axiom-api-1.2.11.jar lib/.
* cp ~/.m2/repository/org/bouncycastle/bcprov-jdk16/1.46/bcprov-jdk16-1.46.jar lib/.


**Security Tip:** when executing the encrypt script, start with a *whitespace* so that this command will not be available in the .bash_history file
and the plain text password can not be seen
