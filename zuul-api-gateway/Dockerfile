# create multi build file
# first take maven base image.
# select workdir
# copy necessary files
# mave install those packages.
# then take open jdk base image
# copy files from build stage
# expose 8080 for documenation
# run the .jar file (application server)

FROM maven as build 
WORKDIR /app 
COPY . .
RUN mvn install 

FROM openjdk:11.0.10-jre
EXPOSE 9999
WORKDIR /app
COPY --from=build /app/target/zuul-0.0.1-SNAPSHOT.jar /app
CMD ["java", "-jar", "zuul-0.0.1-SNAPSHOT.jar"]