pipeline {
	agent any 
	
	stages {
		stage('compile') {
			steps {
				sh 'compile'
				}
			}
			
		stage('Test') {
			steps {
				sh 'test'
				}
			}
			
		stage('clean_package') {
			steps {
				sh 'clean package'
				}
			}
		}
    }	
