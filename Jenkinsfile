pipeline {
    agent any
    stages {
        stage('Run Test'){
            steps{
                bat 'dir'
            }
        }
    }
    post {
        always {
            emailext attachLog: true, attachmentsPattern: 'test_output/**.json', body: 'sample', subject: 'sample', to: 'rahul.sharma@backcountry.com'
        }
    }
}
