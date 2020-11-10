pipeline {
  agent any
  stages {
   stage('GIT Checkout'){
   steps{
     // Clone repo
     git branch: 'master', 
     credentialsId: 'github', 
     url: 'https://github.com/vimalnatarajan/JavaDemo'
   }
   }
   stage('Mvn Package'){
   steps{ 
	  sh "mvn -version"
   }
   }
   // And next stages if you want to define further...
 } // End of stages
} // End of pipeline
