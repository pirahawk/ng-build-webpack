# Ng Build stuff


ng n ngBuildTest -g=false --directory=./src --inlineStyle=false --inlineTemplate=false --routing=true --style=scss -d


ng n ngBuildTest -g=false --inlineStyle=false --inlineTemplate=false --routing=true --style=scss -d


ng n ngBuildTest -g=false --directory=./ --inlineStyle=false --inlineTemplate=false --routing=true --style=scss --skipTests=true -d

ng n ngBuildTest -g=false --inlineStyle=false --inlineTemplate=false --routing=true --style=scss  -d



/////
ng new ng-build-ws --createApplication="false" -d

ng generate application my-second-app --routing=true --style=scss -d





ng g module creditCard --project=my-first-app --flat=false --module=app --routing=true --route="creditCard" -d

ng g component /common-Components/components/someComponent --project=my-first-app --module=common-Components -d


ng build my-first-app




//////////////// WEBPACK


ng n ngBuildWebPack -g=false --inlineStyle=false --inlineTemplate=false --routing=true --style=scss  -d


npm i core-js
npm install @angular-devkit/build-webpack --save-dhtml-loader --save-dev
npm install raw-loader@1.0.0 --save-dev    // NEEDS TO BE V1 for some reason
npm install html-loader --save-dev   // DON'T QUITE NEED THIS!
npm install sass-loader --save-dev
npm install awesome-typescript-loader --save-dev
npm install angular2-template-loader --save-dev



ng run ngBuildWebPack:buildWebPack


"webpackConfig": "webpack.config.js",


Things to do:

# main.ts

```
import 'core-js/es/reflect';
import 'core-js/stable/reflect';
import 'core-js/features/reflect';
```

# app.module.ts

```
import {APP_BASE_HREF} from '@angular/common';

//....

 providers: [
    {provide: APP_BASE_HREF, useValue : '/' }
  ],

```
