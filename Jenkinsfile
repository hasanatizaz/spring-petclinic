pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://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@hasanatizaz/spring-petclinic.git'
                sh 'mvnw package' 
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }
        }
    }
}
