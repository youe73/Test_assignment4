# Test_assignment4

This application is written in Java and the tests are completed with junit5 and maven.  
The (bank) account and creditcard have been tested with unittest, hamcrest, repeated test, dynamic and parameterized tests.



![image](https://user-images.githubusercontent.com/40825848/56477342-ec193580-64a4-11e9-8d3a-735d4dacaecb.png)


![image](https://user-images.githubusercontent.com/40825848/56477414-7f526b00-64a5-11e9-8cbd-6decca4feb05.png)






Decision table is not directly implemented, but as an overall explanation it is conducting a combination of true and false of the outcome of action. 




Below is just an example

@Test
    public void testGetDiscountTTT()
    {
        CreditCard creditCard = new CreditCard(true, true);
         assertEquals(expectedResult, actualResult);
    }
