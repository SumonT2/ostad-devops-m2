pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Read hello.txt') {
            steps {
                script {
                    def content = readFile 'hello.txt'
                    echo "Content of hello.txt: ${content}"
                }
            }
        }
    }
}
