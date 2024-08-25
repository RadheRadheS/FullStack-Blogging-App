pipeline { 
    agent any
    tools {
        maven 'maven3'
        jdk 'jdk17'
    }
    stages {
        
        stage('Compilation of java code') {
            steps {
            sh  "mvn compile"
            }
        }
        
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('Package') {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
