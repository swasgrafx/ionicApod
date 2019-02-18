# ionicApod

NASA's astronomy picture of the day as an Ionic 4 application.

Protect your NASA key by placing it in an exteranal config file. You will need to add this to your providers list in app.module.ts and inject it into the constructor in apod.service.ts. I placed my config file in *~/config*.

*~/config/ng-apod.config.ts*
```ts
export class NgApodConfig{
  key: string = 'xxxxxxxxxxxxxxxx';
}
```

To display videos we will install a [safe-pipe from NPM](https://www.npmjs.com/package/safe-pipe).
```sh
npm install --save safe-pipe
```

## PWA (Optional)

Make it a PWA
```sh
ng add @angular/pwa
```

Be sure to add a link for apple touch as Safari does not yet support linking to icons via manifest files.
```html
<link rel="apple-touch-icon" sizes="192x192" href="assets/icons/icon-192x192.png">
```

PWA Builder offers a [free image generator](https://www.pwabuilder.com/imageGenerator) that allows you to quickly build all recommended icons from a single source file. Be sure to update manifest.webmanifest to match all of your new icons.


