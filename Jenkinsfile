node ('master') {
   def nvmSource = '. ~/.bashrc && '
   stage 'Checkout'
   echo 'Checkout'
   
   // Get some code from a GitHub repository
   git url: 'git@github.com:uniray7/laputa-api.git', credentialsId:'laputa-api-credential'

   stage 'checkkkk'
   sh "${nvmSource} node -v && npm -v"

   stage 'Build'
   sh "${nvmSource} npm install"
}
