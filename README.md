# TPS
usage

This libary use J3D and JOGL to visualize the results. You will need to download J3D package
from the following link
http://jogamp.org/deployment/java3d/1.6.0-pre12/

you will also need JOGL package, which will be availabe at
http://jogamp.org/deployment/jogamp-current/archive/jogamp-all-platforms.7z

copy j3dcore.jar , j3dutils.jar, and vecmath.jar to your Java Extension folder
/Library/Java/Extensions folder, they are j3dcore.jar, j3dutils.jar, vecmath.jar

after unziped jogamp-all-platforms.7z file, you need to copy jogl-all.jar, gluegen-rt.jar in to the /Library/Java/Extension folder (you will need adminstrator previlege to do this)
you also need to add the lib folder in jogamp-all-platforms to your /Libarary/Java/Extension folder

now you are ready to download the TPS package

download the whole directory in to your local computer

cd to the TPS/test

javac -d ../classes ../src/*.java (to compile the source files and put the *.class in classes folder)

javac -d ../classes -cp ../classes TEST.java (to compile the test file)

java -Djava.library.path=/Library/Java/Extensions/lib/macosx-universal/ -cp ../classes/ TEST (run the test)

