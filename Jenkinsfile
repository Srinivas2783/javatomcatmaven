node(Slave1){
    stage('Clone'){
        checkout([$class: 'GitSCM', branches: [[name: '*/SIT-12']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Srinivas2783/javatomcatmaven.git']]])
        echo "Clone"
    }
    stage('Build'){
  bat label: '', script: 'mvn package'
        echo "Build"
    }
    stage('Sonar Analysis'){
        echo "Sonar Analysis"
    }
    stage('Verify Docker Image'){
        echo "Verify Docker Image"
    }
    stage('Deploy to dev'){
        echo "Deploy to dev"
    }
    
    
}
