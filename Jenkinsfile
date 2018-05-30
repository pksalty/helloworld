pipeline {
    agent any
    stages {
        stage('default') {
            agent any
            steps {
                sh 'pylint -f parseable -d I0011, R0801 hello.py | tee pylint.out'
            }
        }
    }
    environment {
        stage = 'default'
    }
}
