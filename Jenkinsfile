pipeline {

   agent any

   stages {
       
       stage ("Creating JSON") {
            steps {
                script{
                    def sldata = readJSON text: '{"name":"John", "age":30, "car":null}'

                    
                    writeJSON(file: 'sl-ib-components.json', json: sldata )
                 }
             }
        }
       
     
