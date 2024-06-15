pipeline {
	agent any
	
	stages {
		stage ('compile') {
			steps {
				sh 'mvn clean compile'
				}
			}
		
		stage ('test') {
			steps {
				sh 'mvn test'
				}
			}
			
		stage ('package') {
			steps {
				sh 'mvn clean package'
				}
			}
		
		stage ('deploy') {
			steps {
				sh 'cp -r /root/.jenkins/workspace/web_app_pipeline/target/maven-web-application.war /root/apache-tomcat-9.0.89/webapps'
				}
			}
		
		}
	}
