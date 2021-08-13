pipeline{
	
	agent any
	environment{
		NEW_VERSION= '1.2.0'	
	}
	
	stages{

		stage("build"){
			steps{
				echo 'Building the app'
				echo " Building using version ${NEW_VERSION}"
				
			}
		}

		stage("test"){
			steps{
				echo ' testing the app'
				script{
					try{
						sh("""#!/bin/bash -l
						set +x
						. \$HOME/vnev/bin/activate
						cd \$WORKSPACE/app
						
						python test.py
						""")
					
					}	
					
					
				}
			}
		}	

		stage("deploy"){
			steps{
				echo 'deploying the app'
			}	
		}

	}
	

}
