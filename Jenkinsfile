node {
checkout scm
def image
def docker = 'docker'

stage('b. Build Image') {
echo 'testingggggg'	
 image = docker.build("dali300/cw2:1.0")
image.push()
}

stage('c. Launch & Test Container') {
def iamge = docker.image("dali300/cw2:1.0").run("-d")
echo "testing: ${iamge.id}"
}

}
