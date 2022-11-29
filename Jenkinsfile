pipeline{
    any agent
    stages{
        stage('1-sysanalys'){
            steps{
                sh 'df -h'
            }
        }
        stage('2-cpuanalysis'){
            steps{
                sh 'lscpu'
            }
        }
        stage('3-memorycheck'){
            steps{
                sh 'fre -g'
            }
        }
        stage('4-os-stat'){
            steps{
                sh 'cat/etc/os-release'
            }
        }
    }
}