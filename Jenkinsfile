pipeline
{
  agent any

  stages{
       stage('build'){

          steps{
            script{
              bat './gradlew build'
            }
          }


       }

       stage('code quality check'){
             steps{
               script{
                       bat "./gradlew sonarqube -Dsonar.host.url=http://localhost:9000 -Dsonar.login=7ce69212e6dd7c108eef4520418ea47664d6c06 -Dsonar.verbose=true"


               }


             }




       }
  }

}
