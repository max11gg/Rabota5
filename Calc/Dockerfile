FROM openjdk:11 
 
RUN apt-get update && apt-get install -y \ 
x11-apps \ 
xauth \ 
libxtst6  
 
ENV DISPLAY=:0 
 
COPY calc.jar /app/ 
 
WORKDIR /app 
 
CMD ["java", "-jar", "calc.jar"]