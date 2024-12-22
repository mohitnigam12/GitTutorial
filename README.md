git clone httpPath

git config --global user.name "userIdGit"

git config --global user.email "emailId"

git add .

git commit -m "anything"

git push -u origin main / git push origin main




DOCKER 


// HelloWorld.java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}


FROM openjdk:17-jdk-slim

WORKDIR /app

COPY HelloWorld.java .

RUN javac HelloWorld.java

CMD ["java", "HelloWorld"]



docker build -t java-hello-world .
docker run java-hello-world


