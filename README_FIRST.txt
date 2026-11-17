EXPERIMENT 9: UNIT TESTING CONTROLLER ENDPOINTS WITH MOCKMVC
============================================================

PROJECT CONTENTS
- pom.xml: Maven configuration and dependencies
- Experiment9MockMvcApplication.java: Spring Boot main class
- MS1Controller.java: GET endpoint for addition
- MS1ControllerTest.java: JUnit 5 + MockMvc test

REQUIREMENTS
- JDK 17 or later
- STS / Eclipse with Spring Tools
- Maven (STS/Eclipse can use its embedded Maven)

IMPORT INTO STS / ECLIPSE
1. Extract this ZIP file.
2. Open STS/Eclipse.
3. Select File > Import.
4. Select Maven > Existing Maven Projects, then Next.
5. Browse to the extracted Experiment_9_MockMvc folder.
6. Select the project and click Finish.
7. Wait for Maven dependencies to download. Internet access may be needed the first time.

RUN THE TEST
1. Expand src/test/java.
2. Open com.example.demo > MS1ControllerTest.java.
3. Right-click the file.
4. Select Run As > JUnit Test.
5. Check the JUnit view. Expected: 1 test, 0 failures, 0 errors.

EXPECTED ASSERTIONS
- Request: GET /ms1/add?a=5&b=10
- HTTP status: 200 OK
- Response body: MS 1.1 - Addition = 15

IMPORTANT
Run MS1ControllerTest as JUnit Test. You do not need to start the full
application to execute this MockMvc web-layer test.

If your lab computer uses a different JDK, set the project JRE to JDK 17
or later: right-click project > Properties > Java Build Path / Java Compiler.
