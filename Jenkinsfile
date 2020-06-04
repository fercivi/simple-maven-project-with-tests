pipeline {
    agent { label { "ec2"}}
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}