# Test_assignment4

This application is written in Java and the tests are completed with junit5 and maven.  
The (bank) account and creditcard have been tested with unittest, hamcrest, repeated test, dynamic and parameterized tests.



![image](https://user-images.githubusercontent.com/40825848/56477342-ec193580-64a4-11e9-8d3a-735d4dacaecb.png)


![image](https://user-images.githubusercontent.com/40825848/56477414-7f526b00-64a5-11e9-8cbd-6decca4feb05.png)

Not all the parameterized tests and dynamic tests served as useful testmethod, probably because of the simplicity in this assignment. Though it is apparent that these tests will be very usefull in tasks where the scope of parameters are widely ranged. 


The boundary analysis has been used as follows. I did not use the equivalence partitioning even it could be useful to test in partitioning groups.

  void getMonthlyInterest() {

        double a = 1000;
        double b = 1001;
        double c = 0;
        double d = -1;
        double e = 99;
        double f = 500;

        Account account = new Account();
        account.GetMonthlyInterest(a);
        assertEquals(5.0,account.GetMonthlyInterest(a));
        assertNotEquals(5.0,account.GetMonthlyInterest(d));
    }


Decision table is not directly implemented, but as an overall explanation it is conducting a combination of true and false of the outcome of action. 

![image](https://user-images.githubusercontent.com/40825848/56485677-4af6a300-64d5-11e9-8d17-deff496728a2.png)


Below is just an example

@Test
    public void testGetDiscountTTT()
    {
        CreditCard creditCard = new CreditCard(true, true);
         assertEquals(expectedResult, actualResult);
    }
