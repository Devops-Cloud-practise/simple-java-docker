# simple-java-docker

make sure you have docker installed.

now create any dir say javabuild

# cd /javabuild
#docker build -t java-image:1.0 -f /javabuild/java-dockerfile .

once image is build create a src dir

#mkdir /javabuild/src

copy hello.java

run the container 

#ls
#java-dockerfile  src
#docker run --rm -v `pwd`/src:/src java-image:1.0

this should print "Hello-world"

/src dir will have Hello-wold.class file will be created. 

Now you can keep on changing the .java file and directly executing by running the container....


