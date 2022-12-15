pipeline {
    agent any
    stages {
        stage('GitIntegration') {
            steps {
               git branch: 'main', url: 'git@github.com:SakivV/pr-python-app.git'
            }
        }
        stage('BuildPython') {
            steps {
                sh 'python3 hello.py'
            }
        }
    }
}
