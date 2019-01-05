
node {
    stage('Checkout'){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'c3d20f97-148b-4cb6-bea8-230e525d664e', url: 'https://github.com/talukder9712/cicd-pipeline-train-schedule-jenkins.git']]])
    }
    
    stage('Build'){
        ./gradlew build
    }

    // checkout scm

    // stage 'Gradle Static Analysis'
    // withSonarQubeEnv {
    //     sh "./gradlew clean sonarqube"
    // }
} 
