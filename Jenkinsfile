//jqglqngl
pipeline {
agent {
label {
		label "built-in-node"
		customWorkspace "/data/project-myapp"
		
		}
		}
		
	stages {
	
		stage ('MAVEN_BUILD') {
		
			steps {
						
						sh "mvn clean package"
			
			}
			
		
		}
		
		stage ('COPY_WAR_TO_Server'){
		
				steps {
						
						sh "cp -r target/LoginWebApp.war /mnt/severs/apache-tomcat-10.1.43/webapps/"

						}
				
				}
	
	
	
	}
		
}
