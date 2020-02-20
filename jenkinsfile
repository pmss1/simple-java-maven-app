def workspace;
node
{
    stage('Checkout'){
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/pmss1/simple-java-maven-app.git']]])
        workspace = pwd()
    }
    stage('Static Code Analysis'){
        echo "Static Analysis done"
    }
    stage('Build'){
        echo "Code Building done"
    }
    stage('Unit Testing'){
        echo "Unit Testing done"
    }
    stage('Delivery'){
        echo "Code Delivery done"
    }
}
