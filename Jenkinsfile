  
node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'vinaykumarnomula') {

        def customImage = docker.build("vinaykumarnomula/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
