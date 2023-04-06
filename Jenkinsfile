pipeline {

    agent any 

    stages {

        stage('GIT CHECKOUT') {

            steps {
                git branch: 'main', url: 'https://github.com/DepressedSaint/XebiaSession-5-6-04-2023.git'
            }
        }
        stage('UNIT TESTING') {
            steps {
                sh 'mvn test'
            }
        }
        stage('INTEGRATION TESTING') {
            steps {
                sh 'mvn verify -DskipUnitTests'
            }
        }
        stage('BUILD') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('STATIC CODE ANALYSIS') {
            steps {
                script {
                    withSonarQubeEnv(credentialsId: 'sonarqubetoken') {
                        sh 'mvn clean package sonar:sonar'
                    }
                }
            }
        } 
    }
}