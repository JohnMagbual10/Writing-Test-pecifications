# Writing-Test-specifications
Writing Test Specifications

A function called "multiplication" that returns the product of the two input numbers.

  1. Expect multiplication of two integers to be correct:
  
  Expect multiplication of (3, 8) to be 24

  2. Expect multiplication of negative two negative and negative five integers to be ten:

     Expect multipliaction of (-2, -5) to be 10

  3. Expect multiplication of two integers negative two and positive six to be negative twelve:
    
     Expect multiplication (-2, 6) to be -12

  4. Expect multiplication of two integers one and five to be five:

  Expect multiplication (1, 5) to be equal to 5

  5. Expect multiplication of zero and two to be zero:

  Expect multiplication (0, 2) to be equal to 0

A function called "concatOdds" takes two arrays of integers as arguments. It should return a single array that only contains the odd numbers, in ascending order, from both of the arrays.
Example: concatOdds([3, 2, 1], [9, 1, 1, 1, 4, 15, -1])
...should result in [-1, 1, 3, 9, 15]
Think about the following; you may need to make assumptions or decisions about the prompt and how the code should behave:
What should happen with unexpected inputs?

1. expect input of non-numerical integer;
   action pop up an error message

2. Expect input of word;
   Action would skip these inputs

3. Expect empty array input;
   Action would return an empty array

4.  Expect Any value inputted other than array
   action would return error message

6. Expect duplicate odd numbers
   Action should function correctly and output would be only uniquely odd numbers



What kinds of unexpected inputs should we worry about?
Empty value is entered
a letter is entered
a symbol is entered
A word is entered 
Inputs are out of expeceted range
Inputs are not odd nunbers


What should happen when there are multiples of the same odd number in the arrays? (Hint: We gave you the answer to this one in the example above.)
should result in [-1, 1, 3, 9, 15]

Functional Tests:
A shopping cart checkout feature that allows a user to check out as a guest (without an account), or as a logged-in user. They should be allowed to do either, but should be asked if they want to create an account or log in if they check out as a guest.
Think about the following; you may need to make assumptions or decisions about the prompt and how the feature should behave:

What should happen if the cart is empty?
1. When a user inputs an empty array, the checkout function will not proceed and the user will be prompted to add an item to cart.
2. When cart is empty, user will not be able to checkout.
3. When cart is empty, user will stay in the same page until cart is filled with items and ready for checkout.

What needs to be shown to the user at each step of check out?
Step 1: cart review will be shown as an ordered list of items user has chosen to checkout.
Step 2: The user will have options to checkout as guest or login. If user chooses to checkout as guest, a prompt will appear providing user to create account or continue as guest.
step 3: If user selects guest checkout, neccessary information will be collected such as shipping address, billing address, and payment details. User will be prompted to create an account.
step 4:  If the user chooses to create an account, user will fill out form and  enter account details such as username, password, email, etc.
Step 5:  If the user chooses to log in, prompt them to enter their login credentials.
Step 6: Summary of the order will be displayed, including items, total cost, shipping details, and payment information. Order Confirmation will be submitted once user clicks the order confirmation button.
Step 7: order information will be sent to users email such as order number, order receipt, and tracking number.
What behaviors of this feature does the prompt miss or gloss over?
1. The prompt does not specify how errors (such as invalid input, network errors, etc.) should be handled during the checkout process.
2. The prompt does not specify how payment processing should be handled, including validation of payment details and communication with payment gateways.
3. There is no mention of order tracking functionality, which allows users to track the status of their orders after checkout.
4. Confirmation emails to users after they complete an order are not addressed
5. The prompt does not specify any limitations or restrictions on guest checkout, such as inability to track orders, access order history, etc.
