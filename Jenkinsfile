pipeline {
    agent any

    stages {
        stage('pull code') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'root', url: 'https://github.com/lilindlzz/hello-world.git']]])
            }
        }
        stage('build project') {
            steps {
                echo "build project"
            }
        }
    }
}
