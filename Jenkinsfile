pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat './mvnw clean' 
            }
        }
		stage('Test') {
			steps {
				bat './mwvnw test'
			}
		}
		stage('Package') {
			steps {
				bat './mvnw package'
			}
		}
		stage('Deploy') {
			steps {
				bat './mvnw deploy'
			}
		}
    }
}
