# ST-JS Bridge parent-pom

## Using to deploy a bridge

in your `~/.m2/settings.xml`
```
<settings>
  <servers>
    <server>
      <id>ossrh</id>
      <username>your-jira-id</username>
      <password>your-jira-pwd</password>
    </server>
  </servers>
  <profiles>
    <profile>
  	  <id>ossrh</id>
  	  <activation>
  	    <activeByDefault>true</activeByDefault>
  	  </activation>
  	  <properties>
  	    <gpg.executable>gpg2</gpg.executable>
  	    <gpg.passphrase>the_pass_phrase</gpg.passphrase>
  	  </properties>
    </profile>
  </profiles>
</settings>
```
