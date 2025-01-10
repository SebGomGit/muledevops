pipeline{  
	agent any 
	
	stages{ 
	
		stage('Build') { 
			steps { 
				bat 'mvn clean deploy' 
			} 
		} 
		
		stage('test') { 
			steps { 
				bat 'mvn test' 
			} 
		} 
		
		stage('deploy') { 
			steps { 
				bat 'mvn clean deploy -DmuleDeploy'
			} 
		} 
	 
	} 
} 
