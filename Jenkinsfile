pipeline {

agent any


stages {


stage('Checkout Code'){

steps{

git branch:'main',
url:'https://github.com/MutahirTayyab/Mutahir_Static_Portfolio.git'

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