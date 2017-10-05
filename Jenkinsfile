node {
    
  stage 'Checkout'

  git 'https://github.com/vish123al/python.git'
        
  stage 'Package Docker image'

  sh 'docker build -t vishaldenge/py .'

  stage 'Publish'
    sh "docker login -u vishaldenge -p 'v!sh@l123' "
  sh 'docker push vishaldenge/py'

}
