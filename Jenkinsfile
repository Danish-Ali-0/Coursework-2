node {
checkout scm
def image
stage('b. Build Image') {
echo 'testingggggg'	
 image = docker.build("dali300/cw2:1.0")
}

stage('c. Launch & Test Container') {
def iamge = docker.container("dali300/cw2:1.0").run("-d")
image.insde {
sh 'curl localhost:8080'
}
}

stage('d. Push to DockerHub') {
}

stage('e. Deploy to kubernetes') {
}

}
