Reproduce:

    yarn install
    ./node_modules/.bin/tsc

```
index.ts(5,33): error TS2345: Argument of type '{ link: any; cache: InMemoryCache; }' is not assignable to parameter of type 'ApolloClientOptions<NormalizedCacheObject>'.
  Types of property 'cache' are incompatible.
    Type 'InMemoryCache' is not assignable to type 'ApolloCache<NormalizedCacheObject>'.
      Types of property 'read' are incompatible.
        Type '<T>(query: ReadOptions) => T | null' is not assignable to type '<T>(query: ReadOptions) => T'.
          Type 'T | null' is not assignable to type 'T'.
            Type 'null' is not assignable to type 'T'.
index.ts(8,9): error TS2554: Expected 1 arguments, but got 0.
node_modules/@types/graphql/subscription/subscribe.d.ts(17,12): error TS2304: Cannot find name 'AsyncIterator'.
node_modules/@types/graphql/subscription/subscribe.d.ts(29,12): error TS2304: Cannot find name 'AsyncIterable'.
node_modules/apollo-cache-inmemory/lib/inMemoryCache.d.ts(5,22): error TS2415: Class 'InMemoryCache' incorrectly extends base class 'ApolloCache<NormalizedCacheObject>'.
  Types of property 'read' are incompatible.
    Type '<T>(query: ReadOptions) => T | null' is not assignable to type '<T>(query: ReadOptions) => T'.
      Type 'T | null' is not assignable to type 'T'.
        Type 'null' is not assignable to type 'T'.
```
