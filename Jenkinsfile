pipeline {
	agent any
	stages{

		stage('build image'){
			steps{
				sh 'docker ps -a'
				sh 'docker build -t achatapnew/jenkinspython .'
			}
			
		}
	}


}
