# typescript-mastery

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
```

# Difference between `any`, `unknown` and `never` type in TypeScript

`any`, `unknown`, and `never` are three special types we use in TypeScript. They behave differently in different situations and cases.



## `any`

The `any` type actually disables type checking. That means, we Can pass any type parameters to a variable, array, or object and it won’t give us an error. When we use `any`, the type can be anything, and it bypasses TypeScript safety.

## `unknown`

There will be cases like: we don't know the type of a parameter at first, but at runtime, we will be able to know the type. In such cases, we use the `unknown` type. The `unknown` type is a safer option compared to `any`.

## `never`

The `never` type is used when there will be cases like a function always throws an error and never returns anything at all or a situation that is impossible.
