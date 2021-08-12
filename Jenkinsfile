pipeline{
	
	agent any
	
	environment{
		New_version=1.2.0	
	}
	stages{

		stage("build"){
			steps{
				echo 'Building the app'
				echo "Building using version ${New_version}"
			}
		}

		stage("test"){
			steps{
				echo ' testing the app'
			}
		}	

		stage("deploy"){
			steps{
				echo 'deploying the app'
			}	
		}

	}
	

}
