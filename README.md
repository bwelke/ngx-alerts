# ngx-alerts

## Installation

To install this library, run:

```bash
$ npm install ngx-alerts --save
```

and then from your Angular `AppModule`:

```typescript
import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';

import { AppComponent } from './app.component';

// Import your library
import { AlertModule } from 'ngx-alerts';

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,

    // Specify your library as an import
    AlertModule.forRoot()
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

Once your library is imported, you can use its components and service in your Angular application:

```xml
<!-- You can now use your library component in app.component.html -->
<h1>
  {{title}}
</h1>
<ngx-alerts></ngx-alerts>
```

Available functions

```
AlertService.info('this is an info alert');
AlertService.danger('this is a danger alert');
AlertService.success('this is a success alert');
AlertService.warning('this is a warning alert');

```


## License

MIT © [Mathijs Blok](mailto:info@mathijsblok.com)
