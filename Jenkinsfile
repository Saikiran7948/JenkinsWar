pipeline {
    agent any   

    stages {
        stage("Git Checkout"){
            steps{
                git credentialsId: 'automation', url: 'https://github.com/saikiran7948/myweb.git'
            }
        }
        stage('build') {
            steps {
                echo "Size ${params.size}"
            }
        }
        stage('deploy') {
            steps {
                echo "Color ${params.color}"
            }
        }
        stage('build-test') {
            steps {
                sh "docker"
                echo "test:color"
            }
        }
    }
}
