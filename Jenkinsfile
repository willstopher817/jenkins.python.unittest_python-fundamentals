timestamps {

    node () {

        stage ('Python-test - Checkout') {
         checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '', url: 'https://github.com/willstopher817/jenkins.python.unittest_python-fundamentals.git']]])
        }
        stage ('Python-test - Build') {
        sh "python unittest discover -s ./src/test/ -p '*_test.py'"
    // Unable to convert a build step referring to "hudson.plugins.powershell.PowerShell". Please verify and convert manually if required.
        }
    }
}