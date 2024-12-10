pipeline {
    agent any

    stages {
        
        stage('Build') {
            steps {
                sh 'mvn install' {}
            }
        }
        stage('Rename') {
            steps {
                sh 'mv target/*.jar target/app.jar'
            }
        }
        stage('Execute') {
            steps {
                sh 'java -jar target/app.jar'
            }
        }
        
    }
}
