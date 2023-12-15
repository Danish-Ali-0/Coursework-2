node {
checkout scm
def image
stage('b. Build Image') {
echo 'testingggggg'	
 image = docker.build("dali300/cw2:1.0")
}

stage('c. Launch & Test Container') {
def iamge = docker.image("dali300/cw2:1.0").run("-d")
echo "testing: ${iamge.id}"
sh "docker push (dali300/cw2:1.0):2.0"
}

}
