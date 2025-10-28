node{
    
    stage('clone'){
        
        git branch: 'feature/2025.10.25', url: 'https://github.com/sahana0321/onlinebookstore.git'
    }
    
     stage('Build'){
         
         bat 'mvn clean install'
    }
    
    stage('Test'){
         
         bat 'mvn clean install'
    }
    
    stage('Artifacts'){
         
         archiveArtifacts artifacts: 'target/*.war', followSymlinks: false
    }
}