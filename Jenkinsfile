pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                script {
                    sh "python -m unittest discover -s ./src/test/ -p '*_test.py'"
                }
            }
        }
    }
}