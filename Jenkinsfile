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

                bat """

                echo Deploying Static Website...

                xcopy /E /I /Y "%WORKSPACE%\\*" "C:\\inetpub\\wwwroot\\Mutahir_Static_Portfolio\\"

                echo Deployment Completed

                """


}

}


}


}