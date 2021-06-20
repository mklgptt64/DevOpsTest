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
         stage ("ssh to ansible server") {
           steps {
             script {
                 sshagent(['5032774f-44b4-44e6-ba78-492b4c3bcbec']) {
                 sh '''
                    ssh -o "StrictHostKeyChecking=no" root@10.54.71.147 < /var/lib/jenkins/workspace/test2/mukul.sh
                    '''
                 }
           }
}
}


    }
    
}
