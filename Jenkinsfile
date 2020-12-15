timestamps {

    node () {

        stage ('Python-test - Checkout') {
         checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '', url: 'https://github.com/willstopher817/jenkins.python.unittest_python-fundamentals.git']]])
        }
        stage ('Python-test - Build') {
            script {
                sh "python unittest discover -s ./src/test/ -p '*_test.py'"
            }
        }
    }
}