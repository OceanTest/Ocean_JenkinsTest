def testnode1 = env.testnode1
def testnode2 = env.testnode2

node('slave1'){
    // Mark the code checkout 'stage'....
    stage('Checkout'){
        // Get some code from a GitHub repository
        git([url: 'https://github.com/OceanTest/Ocean_JenkinsTest.git', branch: 'master'])
        // Mark the code build 'stage'....
    }  
    stage('GetParameter'){
    // Run the program
        println "testnode1 is ${testnode1}"
        println "testnode2 is ${testnode2}"
    }
    // Mark the code run 'stage'....
    stage('Run'){
        // Run the program
        sh script:"ssh root@10.25.132.123 'cd /home/workspace;python3 ocean.py'"
    }
}
