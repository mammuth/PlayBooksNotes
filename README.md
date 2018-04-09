# Play Books Notes
API &amp; Frontend for getting your annotations and quotes from the Google Play Books App.

The app exposes a JSON API for building arbitrary frontends / clients. To be fancy, it also implements a very simple frontend, a web page which displays all your quotes in a slider as seen in the screenshot.

## What is this useful for?
Background info: When using the [Google Play Books app](https://play.google.com/store/apps/details?id=com.google.android.apps.books&hl=en) for reading ebooks, you can annotate sentences. Those annotations and quotes get stored in your Google Drive in an Google Doc which is automatically updated.

Could be used for:
- New Tab page in your browser (using eg. this [Chrome Extension](https://github.com/jimschubert/newtab-redirect/wiki))
- Chromecast Backdrop
- "Quote Of The Day" widget on your phone
- Amazon Alexa Skill

<img width="1680" alt="screen shot 2018-04-08 at 22 11 52" src="https://user-images.githubusercontent.com/3121306/38472156-d7cda50a-3b7b-11e8-9ca0-541296755118.png">

## Usage

### Development
- Run `docker-compose up`
- App will be exposed on localhost:8080

### Deployment
- Modify `docker-compose.prod.yml` according to your needs
- Run `docker-compose -f docker-compose.prod.yml up`
- Think about adding a reverse proxy or use something like Traefik
