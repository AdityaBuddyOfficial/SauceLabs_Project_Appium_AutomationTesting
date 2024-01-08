# SauceLabs_Project_Appium_AutomationTesting

## Overview
This project involves testing a simple E-commerce mobile application using Sauce Labs. The project includes several test cases covering login functionality, shopping cart interactions, and the complete online ordering and checkout process.
## Project Setup
### APK File
Download the mobile application APK file from the following link:
APK File : https://github.com/saucelabs/sample-app-mobile/releases/download/2.2.0/Android.SauceLabs.Mobile.Sample.app.2.2.0.apk
 
### Test Requirements
- Java
- Maven
- Appium
- TestNG
- NodeJs
- Appium Inspector
- Android Studio
- Sauce Labs account (for parallel execution)--> username=standard_user; password=secret_sauce
## Test Cases

### TC#1: Login with Valid username and Password

- Objective: Verify successful login with valid credentials.
- Overview: This test case validates the ability to log in with a valid username and password.
- Steps:
 1. Open the Sauce Labs mobile app.
 2. Enter a valid username and password.
 3. Click on the login button.
 4. Validate that the login is performed successfully.
    
### TC#2: Login with Invalid username or Password

- Objective: Validate the application's response to invalid login attempts.
- Overview: This test case checks the app's behavior when attempting to log in with invalid credentials.
- Steps:
 1. Open the Sauce Labs mobile app.
 2. Enter an invalid username or password.
 3. Click on the login button.
 4. Validate the display of an appropriate error message (Username and password do not match any user in this service).
    
### TC#3: Add Any Item to the Cart

- Objective: Ensure the ability to add items to the shopping cart.
- Overview: This test case adds an item to the cart and validates the displayed details.
- Steps:
 1. Open the Sauce Labs mobile app.
 2. Browse through the items.
 3. Add any item to the cart.
 4. Navigate to the home page.
 5. Validate that the title and price of the item on the home page match the cart.
    
### TC#4: Validate Removing Items from the Cart

- Objective: Verify the ability to remove items from the shopping cart.
- Overview: This test case ensures users can successfully remove items from the cart.
- Steps:
 1. Open the Sauce Labs mobile app.
 2. Add an item to the cart.
 3. Navigate to the cart.
 4. Remove the item from the cart.
 5. Validate that the cart is empty.
    
### TC#5: Online Ordering and Checkout

- Objective: Complete the online ordering and checkout process.
- Overview: This test case covers the end-to-end flow from adding items to the cart to successful checkout.
- Steps:
 1. Open the Sauce Labs mobile app.
 2. Browse through the items.
 3. Add items to the cart.
 4. Navigate to the cart.
 5. Proceed to checkout.
 6. Complete the checkout flow, providing necessary information.(First Name,Last Name,PostalCode)
 7. Validate the final price and success purchase.
    
## Running the Tests

1. Ensure the project dependencies are installed using Maven:
   here are the dependency:-
   <dependencies>
        <!-- https://mvnrepository.com/artifact/io.appium/java-client -->
        <dependency>
            <groupId>io.appium</groupId>
            <artifactId>java-client</artifactId>
            <version>9.0.0</version>
        </dependency>


        <!-- https://mvnrepository.com/artifact/org.testng/testng -->
        <dependency>
            <groupId>org.testng</groupId>
            <artifactId>testng</artifactId>
            <version>7.6.1</version>
            <scope>test</scope>
        </dependency>

    </dependencies>
2. Adjust the Appium server configurations in the test code.
3. Adjust the Appium Inspector to find the locators of the element
4. Using Android Studio to monitor the work Flow
