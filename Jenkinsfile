pipeline{
    agent any
    stages{
        stage('1-script'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'pretei45', url: 'https://github.com/pretei45/appbank.git']])
            }
        }
        stage('2-clonecode'){
            steps{
                sh 'df -h'
            }
        }
        stage('3-memorycheck'){
            steps{
                sh 'free -g'
            }
        }
        stage('4-welcomepage'){
            steps{
                echo "welcome to jenkins"
            }
        }
    }
}