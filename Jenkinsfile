pipeline{
	agent{ docker { image 'maven:3.9.5-ibm-semeru-17-focal'}}
	//agent any

	stages{
		stage('Build'){
			steps{
				sh 'mvn --version'
				echo 'Build'
			}
		}

		stage('Test'){
			steps{
				echo 'Test'
			}
		}

		
		stage('Integration Test'){
			steps{
				echo 'Integration Test'
			}
		}
	}

	post{
		always{
			echo 'I run always'
		}

		success{
			echo 'I run on success'
		}

		failure{
			echo 'I run on failure'
		}
	}
	
}
