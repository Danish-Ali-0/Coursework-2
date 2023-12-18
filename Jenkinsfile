node { 

checkout scm 

def image  

     

    stage('b. Build Image') { 

        echo "Buidling..." 

        image = docker.build("dali300/cw2:1.0"); 

    } 

     

    stage('c. Launch & test Container') { 

        echo "Launching..." 

        def id = docker.image("dali300/cw2:1.0").run("-d") 

        echo "Container ID: ${id.id}" 

	sh 'curl localhost:8080'
    } 

     

    stage('d. Push to DockerHub') { 

        echo "Pushing..." 

        docker.withRegistry('https://registry.hub.docker.com', 'docker') { 

            image.push('2.0') 

        } 

    } 

} 
