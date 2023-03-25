pipeline{
	agent any
	stages{
		stage('1-clone'){
			steps{
				sh 'lscpu'
				sh 'whoami'
			}
		}
		stage('2-systemcheck'){
			steps{
				sh 'sudo systemctl status jenkins'
				sh 'logname'
			}
		}
        stage('3-diskcheck'){
			steps{
				sh 'df -h'
			}
		}
		stage('4-another operation'){
			steps{
				sh 'lsblk'
			}
		}
	}
}