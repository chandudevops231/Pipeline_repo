properties([
    
    parameters([
        choice(choices: ['IL', 'CA'].join("\n"), description: 'select state', name: 'state'),  
        string(defaultValue: 'Chandu', description: 'Enter your name', name: 'Name', trim: false)
       
        ])
        
        ])

if(state=='IL')
{
    
    j_node='master'
}    else{
    
    j_node=w4
}

node(j_node){
    
 stage('Build and package'){
     echo 'generated .war file'
     sleep 10
     powershell 'mvn --version'
     echo "Choice: ${params.state}"
     echo "Choice: ${params.Name}"


 }
     
 stage('deploy code to QA'){
     echo 'deploying .war to QA'
    
}
  
stage('deploy code to prodeuction'){
      echo 'deploying code to production'
  
}
  
}  
