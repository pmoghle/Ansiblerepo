pipeline {
    agent any
    stages{
        stage('s3 bucket create'){
            steps{
                withAWS(credentials:'aws_creds') {
                    sh label: '', script: 'ansible-playbook create_s3.yml'
                }
            }
        }
    }
}
