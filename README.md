# Webshop App Available functionalities:

## General Functionalities:
- Typescript + Javascript + ReactJS + Redux
- NodeJS as backend
- MongoDB as database
- React as frontend
	- Redux to support the app state
- User registration with smtp with gmail and Social sign-in (Facebook and Google)
- Local sign-in functionality with PassportJS JWT strategy
	- Expirable Local Storage to control user login and logouts
- Typescript to provide static typing for better control of data and its types
- Bootstrap4 and page breaks used for responsive design
- Standardized errors and validations

# Views
## Standard home page direction for guests
- Container routes to the 'App'presentational view and shows the home page for guests with Login functionality
- Redux enables synchronized app data state among the web page routes
- Web app has currently automatic login functionalities for the users who has expiring verified localstorage token
	- In case user is already logged in(via local or social signin/out), login functionality disables and a logout functionality appears
- This page also enables users to do basic searches of Books, Toys and other categories and relevant subcategories. Accordingly, it shows the relevant items and controls the store state
- Custom search capability from an open text field
- Enables user favorite products tracking for registered and logged in users
- Enables usert shopping basket tracking and checkout for registered and logged in users

![alt text](https://github.com/mesarikaya/FinalWebShopReactApp/blob/master/snapshots/Capture1.PNG)

## Product page
- Provides details of the clicked product. 
	- Its image
	- Author or producer
	- Description
	- Enables adding to favorites and/or shopping basket

![alt text](https://github.com/mesarikaya/FinalWebShopReactApp/blob/master/snapshots/Capture2.PNG)

## Account Page
- This route enables sign in or sigup functionality
- Sign in is managed by PassportJS JWT strategy which enables Local storage token validation and expiry
- Additional Social login plugins will be enables later on
- Sign up click diverts to the Sign up form page

![alt text](https://github.com/mesarikaya/FinalWebShopReactApp/blob/master/snapshots/Capture3.PNG)

## Favorites Page
- Gives a card list of the selected favorite items for the logged in user
![alt text](https://github.com/mesarikaya/FinalWebShopReactApp/blob/master/snapshots/Capture5.PNG)

## Shopping Basket Page
- Gives a card list of the selected favorite items for the logged in user
![alt text](https://github.com/mesarikaya/FinalWebShopReactApp/blob/master/snapshots/Capture6.PNG)

## Sign up Page
- Provides the sign up form and enables local user registration via using smtp with gmail
- Upon registration sign up is done via using smtp with gmail and it sends a verification email to the user with a token.
Upon verification link click in the sent email, user is directed to 'verify' route. If the token is verified, then user is directed
to the main page and the current state of the store is presented. If not, it stays in the 'account' page.
![alt text](https://github.com/mesarikaya/FinalWebShopReactApp/blob/master/snapshots/Capture4.PNG)



