pipeline {
    agent any

    stages {
        stage ("git checkout") {
         steps {
           git branch: 'main', url: "https://github.com/mklgptt64/DevOpsTest.git" 
           
           
} 
} 
        stage ("run") {
         steps {
           script {
            /*sh 'chmod +x /var/lib/jenkins/workspace/test2/mukul.sh'*/
            sh 'chmod +x /var/lib/jenkins/workspace/test2/mukul.sh'
            sh '/var/lib/jenkins/workspace/test2/mukul.sh'
            
           }
}
}


    }
    
}
