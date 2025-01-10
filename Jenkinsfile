pipeline{  
	agent any 
	
	stages{ 
	
		stage('build') { 
			steps { 
				bat 'mvn clean -DskipTest package' 
			} 
		} 
		
		stage('publish exchange') { 
			steps { 
				bat 'mvn clean deploy' 
			} 
		} 
		
		stage('deploy') { 
			steps { 
				bat 'mvn clean deploy -DmuleDeploy'
			} 
		} 
	 
	} 
} 
