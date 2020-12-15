pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                script {
                    sh "python unittest discover -s ./src/test/ -p '*_test.py'"
                }
            }
        }
    }
}