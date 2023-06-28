pipeline {
    agent any 
    stages {
        stage('Make Virtual Env') { 
            steps {
                withPythonEnv('Python3') {
                    sh 'pipenv install'
                }
            }
        }
    }
}