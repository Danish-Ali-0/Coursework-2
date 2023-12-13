node { 	
checkout scm
	stage ('dockerhub test') {
	echo 'testingggggg'	
	def image = docker.build("dali300/cw2:1.0")
	image.inside {
	sh 'docker ps'	
}
}
}
