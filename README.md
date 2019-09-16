# Developing Microservices in Java 1 - Helidon

Bu proje **Developing Microservices in Java 1 - Helidon** sunumda kullanılan örnek kodlar içermektedir.

 **Developing Microservices in Java 1 - Helidon**

- greet-mp-example
- greet-se-example

# Kurulum

Bu proje Gradle build tool ile oluşturulup Java yazılım dili standartları ile oluşturulmuştur. Proje içerisinde 
gradle wrapper (gradlew) bulunmaktadir ek Gradle kurulum gerekmemektedir ve tercih edilen Gradle destekleyen IDE import edilebilmektedir.

# Build

**Helidon projelerinin JAR üretilmesi:**

    git clone ....
    cd helidon-demo
    ./gradlew build    

# Run
 **Helidon MP**
 
Helidon Microprofile (MP) örneğinin çalıştırılması için
 
    cd greet-mp-example/build/libs
    java -jar greet-mp-example.jar
    
 **Helidon SE**
 
Helidon Standard Edition (SE) örneğinin çalıştırılması için
 
    cd greet-se-example/build/libs
    java -jar greet-se-example.jar
 
 # Test

curl ile serverların test edilmesi

**Greet**  

curl -X GET http://localhost:8080/greet/helidon

**Settings**

curl -X POST http://localhost:8080/greet/settings/OLA

     
# Lisans
   
Foriba Bulut API Java Test Projesi, **Foriba R&D** ekibi tarafından API kullanımını anlatmak için hazırlanmıştır, izinsiz olarak ticari uygulamalarda kullanılması yasaktır.
