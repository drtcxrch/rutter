# rutter

# (External) Platform Support Engineer Technical Assessment

### Overview

In this assessment, you will do 2 things:

1. Play the role of a new Rutter customer and install Rutter Link, our front-end authentication module for connecting to merchant stores.
2. Play the role of a support engineer and respond to a few realistic customer issues during the Rutter implementation.

Overall, this assessment should take 1-2 hours to complete. Your results will be used in the technical interview portion of the onsite.

You can duplicate this entire Notion page as a template, and you are encouraged to add notes as you go through the assignment.

Please communicate freely with eric@rutterapi.com during the interview process - some points are left vague on purpose, and our documentation is not perfect!

### Pre-work (15-30 Minutes)

To be fully prepared to tackle this challenge you should:

1. [Read our documentation](https://docs.rutterapi.com/reference/introduction-to-rutter), specifically:
    1. [Basic concepts](https://docs.rutterapi.com/reference/basic-concepts), [merchant authentication](https://docs.rutterapi.com/reference/merchant-authentication), [API authorization](https://docs.rutterapi.com/reference/authentication) and [connection lifecycle](https://docs.rutterapi.com/reference/connection-lifecycle).
2. Familiarize yourself with REST APIs and how to work with JavaScript-based web applications.

### Task 1: Install & Deploy Rutter (30-45 Minutes)

Pretend you are a new customer who understands Rutter’s value and needs to implement it as soon as possible. Please perform the following actions:

1. Use the [https://dashboard.rutterapi.com/sign-up](https://dashboard.rutterapi.com/sign-up) ****page to sign up for a Rutter account, and in the “Company Name” field, write “Rutter Interview”.
2. After creating your account, follow the [Rutter Tutorial](https://dashboard.rutterapi.com/tutorial), [The React Quickstart](https://docs.rutterapi.com/docs/getting-started) to implement a working version of Rutter Link using the Rutter libraries & documentation provided. Your implementation should open the Rutter Link popup & successfully authenticate a store.
    1. You are free to use whatever tool you prefer to implement Rutter Link. Here is an example [Repl.it](http://Repl.it) that has starter code to implement this assignment: [https://replit.com/@rutterteam/Rutter-Link-Interview-Starter?v=1#style.css](https://replit.com/@rutterteam/Rutter-Link-Interview-Starter?v=1#style.css)
    2. You can use either the Sandbox or the Production environment
3. Using the Rutter Link flow you have implemented, create a new connection by connecting any store. Afterwards, make a call to the [Fetch Connection by Access Token](https://docs.rutterapi.com/reference/fetch-a-connection) endpoint and paste the response of the API call below this text.

    ```jsx
    API_RESPONSE_GOES_HERE
    ```


### Task 2: Help Rutter Customers with their Implementation (30-45 Minutes)

Now, pretend you are working on the Rutter team and helping a new client set up Rutter in their application. Please respond to the following questions in writing (you can pretend they have asked these questions over Slack).

For each question, you should write 2 responses:

1. A response meant to be sent directly to the customer.
2. Your best understanding of what the issue/concern is and best deduction for an approach to resolve / potential solution.

### Situation 1

> Hi Rutter team, we are implementing the Rutter Link process and have run into an issue. After we get the token back from the `onSuccess` callback, we are trying to call the GET /orders endpoint and receiving a 400 error. Can you please help?
>

### Situation 2

> Hi Rutter team, we just connected our first store and are trying to call the API but are getting a 400 response PRODUCT_NOT_READY error. Can you please help us resolve this issue?
>

### Situation 3

> Hi team, our UX team does not like the experience of the Rutter popup flow, and would like to use another method. We saw the [https://docs.rutterapi.com/reference/create-a-connection](https://docs.rutterapi.com/reference/create-a-connection) endpoint and it looks promising. Can this method work for authenticating merchants without using the Rutter popup?
>