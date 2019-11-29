pipeline {

    agent any 
	tools {
		maven "M3"
	}

    stages {

        stage('Build') { 

            steps {

                // Etape Compile
				echo  'Etape compile'
		    		bat 'mvn clean compile'

            }

        }

        stage('Test') { 

            steps {

                // Etape test
				echo 'Etape test 1'

            }

        }

        stage('Packaging') { 

            steps {

                // ceci est un commentaire
				echo 'Etape Packaging' 

                }
		}

        stage('Deploy') { 

            steps {

                // autre commentaire
				echo 'Etape Deploy'

            }

        }

    }

}
