pipeline {
	agent any
	stages{

		stage('build image'){
			steps{
				sh 'docker ps -a'
				#sh 'docker build -t achatapnew/jenkinspython .'
			}
			
		}
		stage('upload image'){
			steps{
				withCredentials([usernamePassword(credentialsId: '451d59f2-101f-4716-948d-00b8659b08b1', passwordVariable: 'password', usernameVariable: 'username')]) {
    			sh 'docker login -u $username -p $password'
}
			}
		}
	}


}
