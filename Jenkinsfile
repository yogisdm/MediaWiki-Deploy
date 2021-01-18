pipeline {
  
  agent any  
  
  stages {
    stage('checkout') {
      steps {
        checkout scm
  	    }
    	}
    
 
    stage('terraform version') {
      steps {
        sh 'terraform --version'
		sh 'terraform plan'
      }
    }
	
    stage('Mediawiki-deploy') {
      steps {
        sh 'terraform apply'
	      
      }
    }

  }
  
  
}