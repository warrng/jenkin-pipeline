pipeline {
    agent any
	environment {
	     test = 'redhat'
	}
	parameters {
	    string(name: "person",defaultValue: "Shivani Warikoo", description: "HOw are you")
		choice(name: "BuildType", choices: "debug\nrelease", description: "chose build type")
    }
    stages {
        stage('run some linux command') {
            steps {
                sh 'date'
				sh 'cal'
            }        
        }
	    stage( 'Check Parameters') {
            steps {
                sh 'echo $person'
            }
		stage( 'Check your choice') {
            steps {
                sh 'echo $BuildType'
            }  
	 }				
   }	
}
 
