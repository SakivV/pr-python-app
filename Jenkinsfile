pipeline {
    agent any
    stages {
        stage('SCMPull') {
            steps {
               git branch: 'main', url: 'git@github.com:SakivV/pr-python-app.git'
            }
        }
        stage('RunPython') {
            steps {
                sh 'python3 hello.py'
            }
        }
    }
}
