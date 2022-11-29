pipeline{
    agent any
    stages{
        stage('1-clonerepo'){
            steps{
                sh 'echo "hello Etech"'
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
    }
}