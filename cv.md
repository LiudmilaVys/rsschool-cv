# Liudmila Vysotskaya
### Software Engineer

***

## Contacts
* e-mail: [liudmila.vys@gmail.com](mailto:liudmila.vys@gmail.com)
* Telegram: [@Liudmila_Vysotskaya](https://t.me/Liudmila_Vysotskaya)
* [LinkedIn](https://www.linkedin.com/in/liudmila-vysotskaya-b5396911b/)

***

## About myself
 Started my career as a sortware engineer at the end of 2014 with Java. After approxiamately 2 yars decided to switch to the world of Front-end. Spent nerly 3 years developing application for people involved in share trading. My responsobility was to build and support page with everyday digest: latest news, rates. In some cases data has been taken from buid-in widgets provided by our team. In others - data has been callected and procesed manually. We had back-end service written on TS, which performed various multiple subrequests for financial data. With all this I would like to say that I have practical experience on a real project, building up UI view as well as backend programming. Since september 2019 I'm at maternity leave. Curretly I'm preparing for getting back at work.

***

## Skills
* TypeScript
* JavaScript
* Cascading Style Sheets (CSS)
* LESS (Stylesheet Language)
* HTML
* Node.js
* Angular 2
* Git

***

## Code example
```
const validate = async (req, res, next) => {
  if (!req.body.login) {
    res.status(BAD_REQUEST).send(messages.loginRequired);
  } else if (!req.body.password) {
    res.status(BAD_REQUEST).send(messages.passwordRequired);
  } else {
    const user = await userService.getByName(req.body.login);
    if (user) {
      const passwordIsValid = await authService.checkCredentials(
        req.body.password,
        user.password
      );
      if (passwordIsValid) {
        next();
      } else {
        res.sendStatus(FORBIDDEN);
      }
    } else {
      res.sendStatus(FORBIDDEN);
    }
  }
};
```
For more information please visit my [GitHub repository](https://github.com/LiudmilaVys/express-REST-service).

***

## Education
Graduated from Belarusian State University of Informatics and Radioelectronics (Software for Information Technologies department) in 2016.

***

## Languages
* Russian - native speaker
* Belarusian - intermediate
* English - B1
* Polish - A2