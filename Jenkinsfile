node('OTE_Agent')  {

    stage('Clone repository') {
        /* Let's make sure we have the repository cloned to our workspace */

        checkout scm
    }

    stage('Build') {
        sh 'docker build . -t hello-world:1.0.0'
    }

    stage('Run') {

        sh 'docker run --rm hello-world:1.0.0'
    }

    
}