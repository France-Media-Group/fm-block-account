# New Account Area Notes
Below, you will find each new section of the **Account Area** and the details of each section.

## Contents
- [Links for testing](#links-for-testing)
- [Your account](#your-account)
- [Your membership](#your-membership)
- [Your details](#your-details)
- - [Details](#details)
- - [Card](#card)
- - [Invoices](#invoices)
- - [Password](#password)
- [Issues](#issues)
- - [Membership - Renewal (Select Option)](#membership---renewal-select-option-will-resolve)
- - [SPOT and Stripe Connection](#spot-and-stripe-connection-cannot-resolve)
- - [Membership - Renewal (Card Payment)](#membership---renewal-card-payment)
- [Test Card Numbers](#test-card-numbers).

## Links for testing
- [Create new Membership](https://staging2.francetoday.com/become-a-member/) (https://staging2.francetoday.com/become-a-member/)
- [Login](https://staging2.francetoday.com/login) (https://staging2.francetoday.com/login)
- [Account Area](https://staging2.francetoday.com/account) (https://staging2.francetoday.com/account)

## Your account
Displays an overview of the account. The e-mail address of the subscriber and the date the account was created are displayed here.

![image info](https://staging2.francetoday.com/test-img/account.png)

## Your membership
Displays the products the subscriber is able to access, and the expiry / renewal dates. 

![image info](https://staging2.francetoday.com/test-img/membership.png)

If a membership is expired, the subscriber will see a message that their membership has expired and a button to renew.

![image info](https://staging2.francetoday.com/test-img/membership2.png)

Clicking on the button will reveal a modal box with the membership options:

![image info](https://staging2.francetoday.com/test-img/membership3.png)

Once the option has been clicked, the subscriber will be taken to the payment page where they will be able to use an existing card, or add a new one:

![image info](https://staging2.francetoday.com/test-img/membership5.png)

## Your details
This section allows the subscriber to update their details, including their name, password, and manage payment cards.

### Details 
The subscriber can update their name. ![image info](https://staging2.francetoday.com/test-img/details1.png)
### Card
The subscriber can manage their payment cards. ![image info](https://staging2.francetoday.com/test-img/details2.png)
### Invoices
The subscriber can view their invoices. ![image info](https://staging2.francetoday.com/test-img/details3.png)
### Password
The subscriber can update their password. ![image info](https://staging2.francetoday.com/test-img/details4.png)

## Issues
Below are the issues that have been found in the new account area.

### Membership - Renewal (Select Option) [WILL RESOLVE]
Currently, there's a problem in `Your membership` (renewal step 2, select membership) where the details of each option are not present.

### SPOT and Stripe Connection [CANNOT RESOLVE]
If the website cannot match the stored `customer_id` with the `customer_id` of Stripe, they will get the following outputs in these specific areas:

#### Details - Card 
The subscriber will see a message that there is an issue retrieving cards for their account. ![image info](https://staging2.francetoday.com/test-img/details5.png)
#### Details - Invoices 
Invoices**: The subscriber will see a message that there is an issue retrieving invoices for their account. ![image info](https://staging2.francetoday.com/test-img/details6.png)
#### Membership - Renewal (Card Payment)
The subscriber will see a message that there is an issue retrieving cards for their account. ![image info](https://staging2.francetoday.com/test-img/membership4.png)

## Test Card Numbers

- `Generic` 4242 4242 4242 4242 | 123 | 10/30
- `3D Secure` 4000 0025 0000 3155 | 123 | 10/30
- `Declined` 4000 0000 0000 0002 | 123  | 10/30

More cards - https://docs.stripe.com/testing?locale=en-GB
