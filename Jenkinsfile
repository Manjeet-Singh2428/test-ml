pipeline {
    agent any
    
    stages {
        stage('Test JDK Version') {
            steps {
                script {
                    def jdkVersion = sh(script: 'java -version 2>&1 | awk -F[\\\"_] \'NR==1{print $2}\'', returnStdout: true).trim()
                    echo "JDK Version: ${jdkVersion}"
                }
                script {
                    sh ``` neofetch
                    time
                    ```
                }
            }
        }
    }
}