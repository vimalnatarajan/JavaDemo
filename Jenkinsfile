pipeline {
  agent any
  stages {
   stage('GIT Checkout'){
    // Clone repo
	git branch: 'master', 
	credentialsId: 'github', 
	url: 'https://github.com/vimalnatarajan/SpringBootDemo'
   
   }
   stage('Mvn Package'){
	   // Build using maven
	   def mvn = tool (name: 'maven3', type: 'maven') + '/bin/mvn'	   
	   sh "${mvn} clean package deploy"
   }
   // And next stages if you want to define further...
 } // End of stages
} // End of pipeline
