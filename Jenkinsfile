node {
checkout scm
	stages {
		stage ('b. Build Image') {
		echo 'testingggggg'	
		def image = docker.build("dali300/cw2:1.0")
		}
		stage('c. Launch & Test Container') {
		}
		stage('d. Push to DockerHub') {
		}
		stage('e. Deploy to kubernetes') {
}
}
}
