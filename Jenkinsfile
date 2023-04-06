pipeline {
    agent any

    stages {
<<<<<<< HEAD
<<<<<<< HEAD


        stage('GIT CHECKOUT'){

            steps{
        git branch: 'main', url: 'https://github.com/delphicarsh20/javacicode.git'
            }

        }
    }
}
=======
        stage('GIT Checkout') {
=======
        stage('GIT CHECKOUT') {
>>>>>>> 50b9707a0290187a481e57b74f255abf56f5b1b3
            steps {
                git branch: 'main', url: 'https://github.com/vishalchauhan91196/java1.git'
            }
        }

        stage('UNIT TESTING') {
            steps {
                sh 'mvn test'
            }
        }

        /*stage('INTEGRATION TESTING') {
            steps {
                sh 'mvn verify -DskipUnitTests'
            }
        }

        stage('MAVEN BUILD') {
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

        stage('QUALITY GATE STATUS') {
            steps {
                script {
                    waitForQualityGate abortPipeline: false, credentialsId: 'sonarqubetoken'
                }
            }
        }

        stage('Upload Artifacts to Nexus'){
            
            steps{

                script{

                    nexusArtifactUploader artifacts: 
                [
                    [
                    artifactId: 'springboot',
                    classifier: '', 
                    file: 'target/Thapar.jar', 
                    type: 'jar'
                    ]
                ], 
                    credentialsId: 'nexuscreds', 
                    groupId: 'com.example', 
                    nexusUrl: '54.209.100.177:8081', 
                    nexusVersion: 'nexus3', 
                    protocol: 'http', 
                    repository: 'java-release', 
                    version: '1.0.0'
                }
            }
        }

        /*stage("Docker Image Build"){

            steps {

                script {
                    sh 'docker image build -t $JOB_NAME:v1.$BUILD_ID .'
                    sh 'docker image tag $JOB_NAME:v1.$BUILD_ID vishalchauhan9/$JOB_NAME:v1.$BUILD_ID'
                    sh 'docker image tag $JOB_NAME:v1.$BUILD_ID vishalchauhan9/$JOB_NAME:latest'
                }
            }
        }

        stage("Push Docker Image to Docker HUB"){

            steps {

                script {
                    
                    withCredentials([string(credentialsId: 'dockerhub_password', variable: 'dockerhub_creds')]) {

                        sh 'docker login -u vishalchauhan9 -p ${dockerhub_creds}'
                        sh 'docker image push vishalchauhan9/$JOB_NAME:v1.$BUILD_ID'
                        sh 'docker image push vishalchauhan9/$JOB_NAME:latest'
                    }
                }
            }
        }*/
    }
<<<<<<< HEAD
}z
>>>>>>> 9ccfc0a600b2a84e1c3b62fe935d9431ca7f00bc
=======
}
>>>>>>> 50b9707a0290187a481e57b74f255abf56f5b1b3
