To restart jenkins after an upgrade:
  brew services restart jenkins
Or, if you don't want/need a background service you can just run:
  /usr/local/opt/openjdk@11/bin/java -Dmail.smtp.starttls.enable=true -jar /usr/local/opt/jenkins/libexec/jenkins.war --httpListenAddress=127.0.0.1 --httpPort=8080

Sample commands:

```bash
Install the latest Weekly version: brew install jenkins
Install a specific Weekly version: brew install jenkins@YOUR_VERSION
Start the Jenkins service: brew services start jenkins
Restart the Jenkins service: brew services restart jenkins
Update the Jenkins version: brew upgrade jenkins
```


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