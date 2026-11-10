pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Docker Version') {
            steps {
                bat '"C:\\Users\\bvnnr\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" --version'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat '"C:\\Users\\bvnnr\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" build -t hello-jenkins .'
            }
        }

        stage('List Images') {
            steps {
                bat '"C:\\Users\\bvnnr\\AppData\\Local\\Programs\\DockerDesktop\\resources\\bin\\docker.exe" images'
            }
        }
    }
}
