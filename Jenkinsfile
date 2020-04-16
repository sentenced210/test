pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo step build'
            }
        }
        stage('Test') {
            steps {
                sh 'echo step test'
            }
        }
        stage('Deploy for testing') {
            when {
                branch 'testing'
            }
            steps {
                sh 'echo testing branch'
            }
        }
        stage('Deploy for production') {
            when {
                branch 'master'
            }
            steps {
                sh 'echo master branch'
            }
        }
        stage('Deploy for setting_jenkins') {
            when {
                branch 'master'
            }
            steps {
                sh 'echo setting_jenkins branch'
            }
        }
    }
}