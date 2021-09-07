pipeline {

   agent any

   stages {
       
       stage ("Creating JSON") {
            steps {
                script{
                    def sldata = readJSON text: '[{ "component_name": "frontend", "buildSessionId": "123" },{ "component_name": "backend", "buildSessionId": "456" }]'
                    
                    writeJSON(file: 'sl-ib-components.json', json: sldata )
                 }
             }
        }
       
      stage('Validate JSON') {
            steps {
                sh "cat sl-ib-components.json | jq ."
         }
      }
   }
}
