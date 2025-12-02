pipeline{
agent any


         stages{

             stage('checkout'){
                   

steps{

git branch: 'master',url:'https://github.com/bharath0155/jenkinstest3.git'


}
}

stage('Build & Test'){

steps{
sh 'echo "Building now"'
sh 'pytest>result.log||true'
sh 'cat result.log'
}
}

stage('deploying'){


steps{

sh 'echo "deploying now"'

}


}







                  }
}

