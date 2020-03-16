# 🚀 Email Automation

## Usuage

Install all the modules

``` npm install ```

## Configure Config.js

```
const credentials = {
  user: "YOUR_EMAIL_ADDRESS,
  pass: "YOUR_PASSWORD"
};
```

## App.js

```
let recepients = [
  {
    email: "email@email.com",
    message: "Hey Ali"
  },
  {
    email: "email@email.com",
    message: "Hey Abbas"
  }
]; // list of recepients

email(recepients); // call method
```

## Run the app

``` node app.js ```

## Response Data

```
{ accepted: [ 'email@gmail.com' ],
  rejected: [],
  envelopeTime: 1121,
  messageTime: 1045,
  messageSize: 269,
  response: '250 2.0.0 OK  1581967133 o16sm1640960pgl.58 - gsmtp',
  envelope: { from: 'email@gmail.com', to: [ 'email@gmail.com' ] },
  messageId: '<7c93b3dc-99f0-de5e-a763-f91494054dad@gmail.com>' }
}

```

## Troubleshoot

Before sending your email using gmail you have to allow non secure apps to access gmail you can do this by going to your gmail settings here.

![Less Secure App Email Automation Realababs Github](https://miro.medium.com/max/1408/1*mRadzlJaSQhBG47VJUTX4w.png)

Once less secure apps is enabled now nodemailer can use your gmail for sending the emails.

## References:

[Bulk Mail](https://nodemailer.com/usage/bulk-mail/)
