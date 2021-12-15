node{
    stage('i am pulling code from github'){
        git credentialsId: 'ffb783d4-2e62-41a2-ac99-7c99d3e113bc', url: 'https://github.com/DevopsPavankumar/jenk-warfile.git'
    }
    
    stage('build the code using maven'){
        sh 'mvn clean install'
    }

    stage('running docker container'){
        sh 'docker run -itd --name JenkinsTwo -p 9050:9050 jenkins/jenkins'

    }
    
}
