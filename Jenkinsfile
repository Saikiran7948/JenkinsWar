pipeline {
    agent any

    environment {
        GIT_REPO = 'hhttps://github.com/Saikiran7948/JenkinsWar.git' // 🔁 Replace with your repo URL
        GIT_BRANCH = 'master' // or 'master' or any branch you want
    }

    stages {
        stage('Clone') {
            steps {
                echo "Cloning from ${env.GIT_REPO}..."
                git branch: "${env.GIT_BRANCH}", url: "${env.GIT_REPO}"
            }
        }

        stage('Build') {
            steps {
                echo "Size ${params.size}"
            }
        }

        stage('Deploy') {
            steps {
                echo "Color ${params.color}"
            }
        }

        stage('Build-Test') {
            steps {
                sh "docker --version"
                echo "test:color"
            }
        }
    }
}
