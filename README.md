# Karate-DSL-API-Testing  

This repository contains examples and resources for API testing using [Karate DSL](https://github.com/karatelabs/karate), a powerful framework for test automation and performance testing.  

## Features  
- BDD-style test scripting  
- Data-driven API testing  
- Seamless JSON and XML handling  
- Easy assertions for request/response validation  
- Reusable scripts for maintainable testing  

## Prerequisites  
- Java (JDK 8 or higher)  
- Maven  

## Getting Started  

1. **Clone the repository**:  
   ```bash  
   git clone https://github.com/Razib-R75/Karate-DSL-API-Testing/edit/main  
   cd Karate-DSL-API-Testing  
   ```  

2. **Run tests**:  
   Use Maven to execute the tests:  
   ```bash  
   mvn test  
   ```  

3. **View Reports**:  
   Test execution generates an HTML report in the `target/karate-reports` directory.  

## Example Test Script  
```feature  
Feature: Sample API Test  

  Scenario: Validate GET Request  
    Given url 'https://jsonplaceholder.typicode.com/posts/1'  
    When method GET  
    Then status 200  
    And match response.id == 1  
```  

## Resources  
- [Karate DSL Documentation](https://github.com/karatelabs/karate)  
- [BDD Testing with Karate](https://karatelabs.github.io/karate/)  

## Contributing  
Feel free to open issues or submit pull requests for improvements or new test cases.  

## License  
This project is licensed under the MIT License.  
```  
