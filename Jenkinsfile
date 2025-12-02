pipeline { 
    agent any 
 
    stages { 
        stage('Checkout') { 
            steps { 
                git branch: 'main', url: 'https://github.com/bharath0155/jenkinstest3.git' 
            } 
        } 
 
        stage('Build & Test') { 
            steps {
                 sh 'echo "Building project..."' 
                sh 'pytest > result.log || true' 
                sh 'cat result.log' 
            } 
        }
        
          stage('Deploy') { 
            steps { 
                sh 'echo "Deploying application..."' 
            } 
        } 
    } 
}

