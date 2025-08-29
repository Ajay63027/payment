@Library('jenkins-shared-library') _

def configMap = [
    project : "roboshop",
    component: "payment"
    appVersion: "1.0.0"
]

if( ! env.BRANCH_NAME.equalsIgnoreCase('main') ){ // if not equals to main
    pythonEKSPipeline(configMap) // by default it will call, call function inside this pipeline
}
else{
    echo "Please proceed with PROD process"
}