pipeline {
    agent any
    stages {
        stage("Checkout") {   
            steps {               	 
                git url: 'https://github.com/jvsocial/Calculator.git'          	 
            }    
        }
        stage('Build') {
            steps {
                sh "mvn compile"  	 
            }
        }
        stage('dummy') {
            // some block
            steps {  	    
                echo 'Hi Dummy'
              
        }
        stage("Unit test") {          	 
            steps {  	 
                sh "mvn test"    
                echo 'Hi Veeshal'
            }
        }
    }
}
