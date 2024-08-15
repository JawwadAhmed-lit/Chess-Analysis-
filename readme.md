# Chess Game Report

Generate classifications for your Chess moves, for free. Tired of being limited to just two free analyses a day? So were we! That's why we decided to build our own tool to analyze chess games without any restrictions. 

<br><br>
Enter a game by its PGN or pick a game from your Chess.com / Lichess.org account and have it analyzed so that you can see where your mistakes and brilliancies are.

## Running Locally
### Prerequisites
- Node.js 20.x runtime or later.
- TypeScript package installed globally.

### Starting the Application
- Download the source code using `git clone` or download as ZIP.
- Open the root directory of the project in a terminal.
- Run `npm i` to install all of the necessary dependencies.
- Create a file called `.env` in the root directory of the project.
- Choose a port for the webserver by adding `PORT=<some port>` to the file.
- If you want to use a CAPTCHA:
    - Add your client secret as `RECAPTCHA_SECRET=<secret>` to the .env file
    - Open `src/public/pages/report/index.html`, find `data-sitekey`, and replace the value with your reCAPTCHA public site key.
- Run `npm start` to compile TypeScript and start the webserver.

### NPM Scripts
- `npm start` - Compiles TypeScript and starts the webserver.
- `npm run build` - Compiles TypeScript.
- `npm run test` - Generates reports from some sample evaluations for classification testing at `src/test/reports`.

## Project Background
This project was born out of frustration with the limitations of existing online chess analysis tools. We were tired of being restricted to just two free analyses per day, so we decided to take matters into our own hands. By creating this tool, we can now analyze as many games as we want, whenever we want, without any limitations.

## Contributors
This project was developed by Raunak Sarmacharya and Jawwad Ahmed.