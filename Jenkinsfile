pipeline {
    agent any
    stages {
        stage('1-Clonecode') {
            steps {
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'Team7-git-id', url: 'https://github.com/Owusu-77/Project_Jenkins.git']])
            }
        }
        stage('2-Builds') {
            steps {
                sh 'df -h'
            }
        }
        stage('3-RunTest') {
            steps {
                sh 'lscpu'
            }
        }
        stage('4-Deploy') {
            steps {
            echo "We are ready to deploy"
            }
        } 
    }
}












