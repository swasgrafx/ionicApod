# ionicApod

NASA's astronomy picture of the day as an Ionic 4 application.

Protect your NASA key by placing it in an exteranal configuration file. You will need to add this to your providers list in app.module.ts and inject it into you constructor in apod.service.ts. I placed mine in *~/config*.

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
