pipeline {
    agent any

    stages {
        stage('pull code') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/${branch}']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'root', url: 'https://github.com/lilindlzz/test.git']]])
            }
        }
        stage('build project') {
            steps {
                echo "build project"
            }
        }
    }
}
