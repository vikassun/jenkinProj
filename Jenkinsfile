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
				stage ("install"){
					steps{
						echo 'testing the application...'
						bat "mvn install -f jenkinProj"
						}
					}
				stage ("test"){
					steps{
						echo 'deploying the application...'
						bat "mvn test -f jenkinProj"
						}
					}
				}
				stage ("package"){
					steps{
						echo 'deploying the application...'
						bat "mvn package -f jenkinProj"
						}
					}
			}
		
