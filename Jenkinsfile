pipeline {
    agent any

    stages {
        stage ('SCM check') {
            steps {
                sh "https://github.com/willstopher817/jenkins.python.unittest_python-fundamentals.git"
            }
        }

        stage ('Build') {
            steps {
                sh "python -m unittest discover -s ./src/test/ -p '*_test.py'"
            }
        }
    }
}