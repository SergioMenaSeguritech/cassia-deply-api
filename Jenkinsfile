pipeline {
    agent any 
    stages {
        stage('Make Virtual Env') { 
            steps {
                withPythonEnv('/usr/bin/python3.8') {
                    sh 'pipenv install'
                }
            }
        }
    }
}