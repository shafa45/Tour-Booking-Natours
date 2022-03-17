<h1 align="center">
  <br>
  <a href="https://bit.ly/369pffj"><img src="https://github.com/shafa45/Tour-Booking-Natours/blob/main/public/img/logo-green-round.png" alt="Natours" width="200"></img></a>
  <br>
  Natours
  <br>
</h1>

<h4 align="center">An awesome tour booking site built on top of <a href="https://nodejs.org/en/" target="_blank">NodeJS</a>.</h4>

 <p align="center">
 <a href="#deployed-version">Demo</a> •
  <a href="#key-features">Key Features</a> •
  <a href="#features-details">Features Details</a> •
  <a href="#demonstration">Demonstration</a> •
  <a href="#how-to-use">How To Use</a> •
  <a href="#api-usage">API Usage</a> •
  <a href="#deployment">Deployment</a> •
  <a href="#build-with">Build With</a> •
  <a href="#to-do">To-do</a> •
  <a href="#installation">Installation</a> • 
  <a href="#known-bugs">Known Bugs</a> • 
  <a href="#future-updates">Future Updates</a> • 
  <a href="#acknowledgement">Acknowledgement</a>
</p>

## Deployed Version

Live demo (Feel free to visit) 👉 : https://bit.ly/369pffj

## Key Features

- Authentication and Authorization
  - Login and logout
- Tour
  - Manage booking, check tours map, check users' reviews and rating
- User profile
  - Update username, photo, email, and password
- Credit card Payment

## Features Details

- [Users](#users)
- [Tours](#tours)
- [Bookings](#bookings)
- [Reviews](#reviews)
- [Favorite Tours](#favorite-tours)
- [Notice](#notice)

## Users

- Users can sign up with the application.
- Users can log into the application.
- Users can log out of the appication.
- Users can update their password.
- Users can reset their password
- Users can update their general information.
- Users can see their profile page.
- A user can be either a regular user or an admin or a lead-guide or a guide.
- When you sign up, you are a regular user by default.

## Tours

- Tours can be created by an admin user or a lead-guide.
- Tours can be seen by every user.
- Tours can be updated by an admin user or a lead-guide.
- Tours can be deleted by an admin user or a lead-guide.

## Bookings

- Only regular users can book tours (make a payment).
- Regular users can not book thesame tour twice.
- Regular users can see all the tours thay have booked.
- An admin user or a lead-guide can see every booking on the app.
- An admin user or a lead-guide can delete any booking.
- An admin user or a lead-guide can create a booking (manually, without payment).
- An admin user or a lead-guide can not create a bookng for thesame user twice.
- An admin user or a lead-guide can edit any booking.

## Reviews

- Only regular users can write reviews for tours which they have booked.
- All users can see the reviews of each tour.
- Regular users can edit and delete their own reviews.
- Regular users can not review thesame tour twice.
- An admin can delete any review.

## Demonstration

#### Home Page :

![natoursHomePageonline-video-cutt](https://user-images.githubusercontent.com/58518192/72606801-7ebe0680-3949-11ea-8e88-613f022a64e5.gif)

#### Tour Details :

![tourOverviewonline-video-cutterc](https://user-images.githubusercontent.com/58518192/72606859-a0b78900-3949-11ea-8f0d-ef44c789957b.gif)

#### Payment Process :

![paymentprocess-1-ycnhrceamp4-7fW](https://user-images.githubusercontent.com/58518192/72606973-d9eff900-3949-11ea-9a2e-f84a6581bef3.gif)

#### Booked Tours :

![rsz_bookedtours](https://user-images.githubusercontent.com/58518192/72607747-6a7b0900-394b-11ea-8b9f-5330531ca2eb.png)

#### User Profile :

![rsz_userprofile](https://user-images.githubusercontent.com/58518192/72607635-44edff80-394b-11ea-8943-64c48f6f19aa.png)

#### Admin Profile :

![rsz_adminprofile](https://user-images.githubusercontent.com/58518192/72607648-4d463a80-394b-11ea-972f-a73160cfaa5b.png)

## How To Use

### Book a tour

- Login to the site
- Search for tours that you want to book
- Book a tour
- Proceed to the payment checkout page
- Enter the card details (Test Mood):
  ```
  - Card No. : 4242 4242 4242 4242
  - Expiry date: 02 / 22
  - CVV: 222
  ```
- Finished!

### Manage your booking

- Check the tour you have booked in "Manage Booking" page in your user settings. You'll be automatically redirected to this
  page after you have completed the booking.

### Update your profile

- You can update your own username, profile photo, email and password.

## API Usage

Before using the API, you need to set the variables in Postman depending on your environment (development or production). Simply add:

```
- {{URL}} with your hostname as value (Eg. http://127.0.0.1:3000 or http://www.example.com)
- {{password}} with your user password as value.
```

Check [Natours API Documentation](https://documenter.getpostman.com/view/8689170/SVmzvwpY?version=latest) for more info.

## Deployment

The website is deployed with git into heroku. Below are the steps taken:

```
git init
git add -A
git commit -m "Commit message"
heroku login
heroku create
heroku config:set CONFIG_KEY=CONFIG_VALUE
parcel build ./public/js/index.js --out-dir ./public/js --out-file bundle.js
git push heroku master
heroku open
```

You can also changed your website url by running this command:

```
heroku apps:rename natours-users
```

## Build With

- [NodeJS](https://nodejs.org/en/) - JS runtime environment
- [Express](http://expressjs.com/) - The web framework used
- [Mongoose](https://mongoosejs.com/) - Object Data Modelling (ODM) library
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) - Cloud database service
- [Pug](https://pugjs.org/api/getting-started.html) - High performance template engine
- [JSON Web Token](https://jwt.io/) - Security token
- [ParcelJS](https://parceljs.org/) - Blazing fast, zero configuration web application bundler
- [Stripe](https://stripe.com/) - Online payment API
- [Postman](https://www.getpostman.com/) - API testing
- [Mailtrap](https://mailtrap.io/) & [Sendgrid](https://sendgrid.com/) - Email delivery platform
- [Heroku](https://www.heroku.com/) - Cloud platform

## To-do

- Review and rating
  - Allow user to add a review directly at the website after they have taken a tour
- Booking
  - Prevent duplicate bookings after user has booked that exact tour, implement favourite tours
- Advanced authentication features
  - Signup, confirm user email, login with refresh token, two-factor authentication
- And More ! There's always room for improvement!

## Installation

You can fork the app or you can git-clone the app into your local machine. Once done that, please install all the
dependencies by running

```
$ npm i
set your env variables
$ npm run watch:js
$ npm run build:js
$ npm run dev (for development)
$ npm run start:prod (for production)
$ npm run debug (for debug)
$ npm start
Setting up ESLint and Prettier in VS Code 👇
$ npm i eslint prettier eslint-config-prettier eslint-plugin-prettier eslint-config-airbnb eslint-plugin-node
eslint-plugin-import eslint-plugin-jsx-a11y  eslint-plugin-react --save-dev
```

## Acknowledgement

- This project is part of the online course I've taken at Udemy. Thanks to Jonas Schmedtmann for creating this awesome course! Link to the course: [Node.js, Express, MongoDB & More: The Complete Bootcamp 2019](https://www.udemy.com/course/nodejs-express-mongodb-bootcamp/)
