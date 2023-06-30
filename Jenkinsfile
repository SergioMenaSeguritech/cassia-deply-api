pipeline {
    agent any 
    stages {
        stage('Make Virtual Env') { 
            steps {
                withPythonEnv('/usr/bin/python3.8') {
                    sh 'pipenv --python /usr/bin/python3.8 install'
                    sh 'pipenv --python /usr/bin/python3.8 run uvicorn main:app --reload'
                }
            }
        }
    }
}