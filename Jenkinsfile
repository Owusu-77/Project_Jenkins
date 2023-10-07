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
         stage('4-Security_Check') {
            steps {
              sh 'bash -x /var/lib/jenkins/workspace/Team7_project01/pipeline.sh'  
            }
    }
    }
}












