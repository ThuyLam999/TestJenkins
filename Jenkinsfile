node { 
    stage ('Checkout SCM') { 
        git branch: "main", url: ''
    }
    stage ('Install node modules') { 
        sh "npm install"
    }
    stage ('Test') { 
        sh "npm run test-headless"
    }
    stage ('Build') { 
        sh "npm run build --prod"
    }         
 }