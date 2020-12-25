* Start Date: 2020-12-25
* Target Major Version: 1.x

# Summary

Write the deployment logic itself using OCM, we need a "OCM Project" to build a cli type "OCM App".

# Basic Example

src/Cli/HelloWorld.ts

```ts
import * as Biz from '@ocmts/biz';

@Biz.published
export class HelloWorld extends Biz.Command {
  public run() {
    console.log('hello world');
  }
}
```

run it via

```sh
ocm start main-svc
```

