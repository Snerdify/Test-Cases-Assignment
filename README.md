# Test-Cases-Assignment
Generating test cases using Gemini 

Run the notebook in collab. 
The collab notebook contains the Python program that utilizes Google Gemini to
generate manual test cases based on up to 5 screenshots of a user journey in amazon.
1. Reading the screenshots in python .
2. Using the Gemini [1.5-flash , 1.5-flash-8b , 1.5-flash-002](given which one is available) to generate test cases in mentioned format
3. 3 test cases per image generated 



INPUT:
The input-images contain 5 screenshots of amazon website . 
The screenshots include :
1. amazon-home : The home page of amazon
2. amazon-search : The home page whilst searching for a product
3. product-details: The details of the product after the user clicks on the product of choice
4. add-to-cart : The sidebar where the user can now add the product to the cart
5. confirmation: The confirmation that the product is now added to the cart . 


REQUIREMENT:
Each generated test case will contain:
1. Title: A short and descriptive name for the test case.
2. Objective: A clear purpose of the test case (e.g., verifying user interactions, UI elements,
etc.).
3. Steps: A series of steps, where each step includes:
○ Action: What the user is supposed to do (e.g., click a button, enter text).
○ Data (optional): The input data required for the step.
○ Expected Result: What the expected outcome of the step should be.
This is as per requirements of the assignment . 


OUTPUT:
The structured json output for the test cases which is generated using a python is stored in output-files folder . This file can also be directly generated after running the code in collab notebook . 



