pipeline {
    agent { label 'agent-1' }
    
    tools {
        maven 'maven 3.9'
        jdk 'jdk17'
    }

    stages {
        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
