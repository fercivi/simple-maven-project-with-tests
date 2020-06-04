pipeline {
    agent { node { label 'ec2' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn -B -ntp -Dmaven.test.failure.ignore verify'
            }
            junit '**/target/surefire-reports/TEST-*.xml'
        }
    }
}