pipeline {
	agent any 
	
	stages {
		stage('compile') {
			steps {
				sh 'mvn compile'
				}
			}
			
		stage('Test') {
			steps {
				sh 'mvn test'
				}
			}
			
		stage('clean_package') {
			steps {
				sh 'mvn clean package'
				}
			}
		}
    }	
