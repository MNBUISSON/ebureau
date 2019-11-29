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
		    		bat 'mvn clean test'

            }

        }

        stage('Packaging') { 

            steps {

                // ceci est un commentaire
				echo 'Etape Packaging' 
		    		bat 'mvn clean package'

                }
		}

        stage('Deploy') { 

            steps {

                // autre commentaire
				echo 'Etape Deploy'
				bat copy C:\opt\Jenkins\workspace\ebureauPipeline\target\ebureau.war C:\Program Files\"Apache Software Foundation"\Tomcat 9.0\webapps\ebureau.war 
		    		echo "finished"
            }

        }

    }

}
