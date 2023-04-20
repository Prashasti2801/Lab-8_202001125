# Lab-8_202001125

## Unit Testing with JUnit

#### Lab Exercises


##### Create a new Eclipse project
![image](https://user-images.githubusercontent.com/75677179/233335033-0eb61471-6cb2-4ece-a280-c757e992dd3f.png)


##### Within the project create a package and Create a class for a Boa.
![image](https://user-images.githubusercontent.com/75677179/233335310-ab3781d0-8078-4e7e-bb97-b1767ea24dfb.png)


##### Follow the instructions in the JUnit tutorial in the section “Creating a JUnit Test Case in Eclipse”. You’ll be creating a test case for the class Boa. When you’re asked to select test method stubs, select both isHealthy() and fitsInCage(int).

Created a class in the package - class name - Boa and junit test case file - BoaTest
Created junit test case for class Boa - BoaTest and for test method stubs, select both isHealthy() and fitsInCage(int).

    package lab8;

    public class Boa {
      private String name;
      private int length; // the length of the boa, in feet
      private String favoriteFood;

      public Boa (String name, int length, String favoriteFood){
        this.name = name;
        this.length = length;
        this.favoriteFood = favoriteFood;
      }
      // returns true if this boa constrictor is healthy
      public boolean isHealthy(){
        return this.favoriteFood.equals("granola bars");
      }

      // returns true if the length of this boa constrictor is
      // less than the given cage length
      public boolean fitsInCage(int cageLength){
        return this.length < cageLength;
      }
      }
      
![image](https://user-images.githubusercontent.com/75677179/233336310-f902d534-7301-4db4-83c1-3c79783b7c13.png)

##### Stubs for two test methods and Unit tests

![image](https://user-images.githubusercontent.com/75677179/233335451-f7b03361-fa96-4df2-9d77-c2e2209bd8bf.png)


##### Run your tests

![image](https://user-images.githubusercontent.com/75677179/233339373-0990a616-c8ae-4e53-a1c4-6a5dd83e66ac.png)

##### Add a new method to the Boa class, with this purpose and signature:

Adding the following code to the Boa class:

    // produces the length of the Boa in inches
    public int lengthInInches(){
      return this.length*12;
    }
    
![image](https://user-images.githubusercontent.com/75677179/233339749-9d04e411-a4e1-4adc-a643-f4dfb78cd0af.png)
