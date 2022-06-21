pipeline {
		agent any

		stages {
				stage ('git repo & clean'){
					steps{
						echo 'building the application...'
						bat "rmdir /s /q jenkinProj"
						bat "git clone https://github.com/vikassun/jenkinProj.git"
						}
					}
				stage ("test"){
					steps{
						echo 'testing the application...'
						}
					}
				stage ("deploy"){
					steps{
						echo 'deploying the application...'
						}
					}
				}
		}
