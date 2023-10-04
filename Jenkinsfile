pipeline {
    agent any
    stages {
        stage('1-Clonecode') {
            steps {
                checkout(
                    scm: [$class: 'GitSCM', branches: [[name: '*/main']],
                    doGenerateSubmoduleConfigurations: false,
                    extensions: [],
                    submoduleCfg: [],
                    userRemoteConfigs: [[credentialsId: 'Team7-git-id', url: 'https://github.com/Owusu-77/Project_Jenkins.git']]]
                )
            }
        }
        stage('2-Build') {
            steps {
                sh 'df -h'
            }
        }
        stage('3-RunTest') {
            steps {
                sh 'lscpu'
            }
        }
    }
}












