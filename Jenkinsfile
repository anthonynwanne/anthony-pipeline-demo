pipeline{
    agent any
    stages{
        stage('1-clonerepo'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/anthonynwanne/anthony-pipeline-demo.git']]])
            }
        }
        stage('2-sysanalysis'){
            steps{
                sh 'df -h'
            }
        }
        stage('3-cpu stats'){
            steps{
                sh 'lscpu'
            }
        }
        stage('4-os stats'){
            steps{
                sh 'cat /etc/os-release'
            }
        }
        stage('5-securitycheck'){
            steps{
                sh 'bash -x /var/lib/jenkins/workspace/anthony-pipeline-demo/security.sh'
            }
        }
    }
}