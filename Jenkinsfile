node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'aa0a6adb-36db-4173-b23f-9784f7c118d9') {

        def customImage = docker.build("grav")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
