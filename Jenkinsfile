pipeline{
	agent any
	
	environment {
		PATH = "${PATH}:D:/Krishna/Binaries/apache-maven-3.6.0-bin/apache-maven-3.6.0/bin/"
    }
    
    stages{
		stage('SCM - Checkout'){
			steps{
            git credentialsId: 'git_Credentials', url: 'https://github.com/harikrishna12334/sample-project-maven-master.git'
					}
		}
  stage('Maven Build LifeCycle'){
			steps{
           bat "mvn clean compile"
					}
		}
}
}
