pipeline {
    agent any
	environment {
	     test = 'redhat'
	}
	parameters {
	    string(name: "person",defaultValue: "Shivani Warikoo", description: "How are you")
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
		    }				
	    }	
}
 
