"# product-api" 
mvn -DmuleDeploy deploy -Dap.client_id=X -Dap.client_secret=X -Dap.ca.client_id=X -Dap.ca.client_secret=X -Dencrypt.key=X -Ddeployment.env=test
mvn -DmuleDeploy deploy -Dap.client_id=organizationClientId -Dap.client_secret=organizationSecret -Dap.ca.client_id=connectedAppDeploymentclientId -Dap.ca.client_secret=connectedAppDeploymentSecret -Dencrypt.key=secretDecryptionKey -Ddeployment.env=test
mvn install:install-file -Dfile=parent-pom/pom.xml -DpomFile=parent-pom/pom.xml
	
	<server>
      <id>anypoint-exchange-v3</id>
      <username>~~~Client~~~</username>
      <password>myClientId~?~mySecret</password>
    </server>
	exchange contributor connected app creds--->
	<server>
      <id>anypoint-exchange-v3-student-deployment</id>
      <username>~~~Client~~~</username>
      <password>connectedAppWithEnvDeployAndViewPermissionsClientId~?~connectedAppWithEnvDeployAndViewPermissionsClientIdSecret</password>
    </server>