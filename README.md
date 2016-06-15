# crypto-encrypt-util
custom util to get encrypted password for WSO2

### How to build and run
run `mvn clean install`

run the *encrypt* script as follows

`./encrypt <plainTextPassword> <keystoreFilePath> <keystoreFilePassword> <certificateAlias>`

**Security Tip:** when executing the encrypt script, start with a *whitespace* so that this command will not be available in the .bash_history file
and the plain text password can not be seen
