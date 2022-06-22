pipeline {
    agent { label 'terraform' }
    
    tools {
        terraform 'terraform'
    }
    
    stages {
        stage('terraform init') {
            steps {
                sh label: 'terraform', script: 'terraform init'
            }
        }
        
        stage('terraform apply') {
            steps {
                sh label: 'terraform', script: 'terraform apply -auto-approve'
            }
        }
    }
}
