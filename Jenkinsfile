pipeline{
	agent{ docker { image 'maven:3.6.3'}}
	//agent any

	stages{
		stage('Build'){
			steps{
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
