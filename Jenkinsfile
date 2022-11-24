pipeline {
    agent any

    stages {
        stage('Chekout'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: '2665d0f0-f5fa-4271-9ae8-6a9fb711444f', url: 'https://github.com/gineszamorac/calculadora_devops']]])
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
