# Tutorial Assessment

1. In the top-down service, can the client use `getEmployee`, `updateEmployee` methods? Please explain.

   Yes, the client can use `getEmployee`, `updateEmployee`, and any other methods specified in the service endpoint interface in the top-down service. These methods are established within the service endpoint interface through `wsimport` based on the WSDL file. The implementation of these methods is governed by the web service implementation class, which is also established from the WSDL file.

2. If we want the client connected to the bottom-up web service to use `countEmployees` method, what modification should we do in the `EmployeeService.java` and `EmployeeServiceImp.java`?

   To allow the client's access to the `countEmployees` method in the bottom-up web service, we need to add the `@WebMethod` annotation to the method in the `EmployeeService` interface, as follows:

   ```java
   @WebMethod
   int countEmployees();
   ```

   Then, we will have to implement this method in the `EmployeeServiceImpl` class, which fetches the count of `employeeRepositoryImpl`:

   ```java
   @WebMethod
   public int countEmployees() {
     return employeeRepositoryImpl.count();
   }
   ```

3. What is GlassFish?

   **GlassFish** is an open-source application server that supports the Java Platform, Enterprise Edition (Java EE) standard. It provides a platform for developing and deploying enterprise applications, web services, and microservices. Additionally, it serves as the reference implementation of Java EE, ensuring that it fully adheres to Java EE standards specifications and passes the Java EE compatibility tests. The Eclipse Foundation supports GlassFish through the Eclipse GlassFish project. Its Wikipedia page can provide more information [here](https://en.wikipedia.org/wiki/GlassFish), and the source code can be found on GitHub [here](https://github.com/javaee/glassfish).
