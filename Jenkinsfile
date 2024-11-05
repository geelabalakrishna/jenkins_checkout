pipeline {
    agent any
    stages {
        stage('Checkout App') {
            steps {
                // Checkout the main application repository (app)
                checkout([$class: 'GitSCM', 
                    branches: [[name: '*/dev']], 
                    userRemoteConfigs: [[url: 'https://github.com/geelabalakrishna/app.git']]
                ])

                sh 'ls -al'
            }
        }
}
