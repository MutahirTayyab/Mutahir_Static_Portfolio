pipeline {

agent any


stages {


stage('Checkout Code'){

steps{

git branch:'main',
url:'YOUR_GITHUB_REPO'

}

}



stage('Deploy Website Files'){

steps{

bat '''

xcopy /E /I /Y ^
C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Mutahir_Static_Portfolio\\* ^
C:\\inetpub\\wwwroot\\Mutahir_Static_Portfolio\\

'''

}

}


}


}