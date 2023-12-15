node { 	
checkout scm
#	agent { 
#		docker { image 'node:6.14.2' }
#		}
	stages {
		stage ('dockerhub test') {
		echo 'testingggggg'	
		def image = docker.build("dali300/cw2:1.0")
#			image.inside {
#				sh 'curl localhost:8080'	
#			}
}
}
}
