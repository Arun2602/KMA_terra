pipeline {
    agent any
    tools{
        terraform "terraform"
    }
    
    stages {
        stage('terraform init') {
            steps {
                sh label: '', script: 'terraform init'
            }
        }
        
        stage('terraform apply') {
            steps {
                sh label: '', script: 'terraform apply --auto-approve'
            }
        }
    }
}
