pipeline{
	any agent
	stages{
		stage('1-clone repo'){
			steps{
				sh 'pwd'
			}
		}
		stage('2-merge pull request'){
			steps{
				sh 'whoami'
			}
		}
		stage('3-check pipeline sync'){
			steps{
				sh 'df -h'
			}
		}
		stage('4-deploy to dev'){
			steps{
				sh 'free -g'
			}
		}
		stage('5-uat test'){
			steps{
				sh 'du -h'
			}
		}
		stage('6-deploy to prod'){
			steps{
				sh 'free -m'
			}
		}
		stage('final-continuous int'){
			steps{
				sh 'ls'
			}
		}
	}
}