pipeline {
    agent any 
    stages {
        stage('Make Virtual Env') { 
            steps {
                withPythonEnv('/usr/bin/python3.8') {
                    sh 'pipenv install'
                    sh 'pipenv run uvicorn main:app --reload'
                }
            }
        }
    }
}