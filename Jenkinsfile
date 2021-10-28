pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mvnw package' 
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }
        }
    }
}