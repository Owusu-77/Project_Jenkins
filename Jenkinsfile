pipeline{
    agent any
    stages{
        stage(1-Clonecode ){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'Team7-git-id', url: 'https://github.com/Owusu-77/Project_Jenkins.git']])
            }
        }
        stage(2-Build Artifact){
            steps{
                sh 'df -h'
            }
        }
        stage(3-Run Test){
            steps{
                sh 'lscpu'
            }
        }
    }
}