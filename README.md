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

Make it a PWA
```sh
ng add @angular/pwa
```
