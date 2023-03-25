pipeline{
	agent any
	stages{
		stage('1-clone'){
			steps{
				checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/Etech-consulting-llc/rudolph-team5']])
			}
		}
		stage('2-systemcheck'){
			steps{
                sh 'logname'
			}
		}
        stage('3-diskcheck'){
			steps{
				sh 'df -h'
			}
		}
		stage('4-another-operation'){
			steps{
				sh 'lsblk'
			}
		}
	}
}
