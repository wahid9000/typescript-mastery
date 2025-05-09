# typescript-mastery : Blog Posts

# keyof Operator and its Use in TypeScript

The `keyof` operator can be used in various ways in TypeScript. It is versatile and can be implemented in many practical TypeScript pattern problems.

The `keyof` operator is a **type operator** by which we can get the **union of the keys** from a given type.

## Example

```typescript
type Home = {
  sleep: string;
  eat: string;
}

type Home2 = keyof Home; // output: ‘sleep’ | ‘eat’

The Home2 will now include the union of all keys of type Home. We did that using the keyof operator.
