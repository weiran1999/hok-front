pipeline
{
  agent any

  stages {

      stage('Build')
      {
        steps {
          sh" npm install "
          sh" npm run build "
        }
      }

      stage('Deploy')
     {
      steps {
         sh" docker-compose down "
         sh" docker-compose up --build -d "
      }
    }
  }
}
