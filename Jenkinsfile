pipeline{
	agent{ docker { image : 'maven3.6.3'}}
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
