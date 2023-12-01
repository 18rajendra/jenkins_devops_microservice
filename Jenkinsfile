pipeline{
	//agent{ docker { image 'maven:3.9.5'}}
	agent any

	stages{
		stage('Build'){
			steps{
				//sh 'mvn --version'
				echo 'Build'
				echo "PATH - $PATH"
				echo "BUILD_NUMBER - $BUILD_NUMBER"
				echo "BUIILD_ID - $BUILD_ID"
				echo "JOB_NAME - $JOB_NAME"
				echo "BUILD_TAG - $BUILD_TAG"
				echo "BUILD_URL - $BUILD_URL"
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
