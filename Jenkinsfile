pipeline {
    agent any 
    stages {
        stage('Make Virtual Env') { 
            steps {
                withPythonEnv('python3') {
                    sh 'pipenv install'
                }
            }
        }
    }
}