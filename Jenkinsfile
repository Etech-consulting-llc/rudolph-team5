pipeline{
	agent any
	stages{
		stage('1-clone'){
			steps{
				checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'rnfor', url: 'https://github.com/Etech-consulting-llc/rudolph-team5.git']])
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