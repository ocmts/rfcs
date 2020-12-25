* Start Date: 2020-12-25
* Target Major Version: 1.x

# Summary

Minimal API to get data in and out of the cloud, without authentication.

# Basic Example

```ts
import * as Biz from '@ocmts/biz';

@Biz.published
export class Product extends Biz.ActiveRecord {
  public name: string;
  public price: number;
}
```

# Motivation

Define the database table in TypeScript class, so we can query it from frontend in a typesafe way without any hassle. 
No backend api controller needed, no extra frontend model class needed.
