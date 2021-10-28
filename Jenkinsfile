pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
            	git 'https://github.com/hasanatizaz/spring-petclinic.git'
                sh 'mvnw package' 
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }
        }
    }
}
