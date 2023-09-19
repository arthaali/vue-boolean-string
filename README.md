# Vue-boolean-string

Issue with Vue Casting Empty Strings to `true` for `boolean | string` Props

## Summary
Vue.js currently exhibits behavior where it casts empty strings to `true` when handling props of type `boolean | string`. This issue is problematic because it contradicts the expected behavior of preserving empty strings, especially when there is a need for special handling of empty strings within components.

Details:
- Type Definition: Consider a prop defined as `value: boolean | string;`. Vue.js is currently converting empty strings to `true` when passed as props, which may lead to unintended behavior and conflicts with component-specific logic designed to handle empty strings differently.

- Type Order Implications: The order in which the prop types are defined (boolean before string or vice versa) affects the return type, further exacerbating the problem. This inconsistency in return types based on type order adds unnecessary complexity to Vue.js component development and can lead to hard-to-debug issues.

## Project setup
```
pnpm install
```

### Compiles and hot-reloads for development
```
pnpm run dev
```

### Compiles and minifies for production
```
pnpm run build
```

### Lints and fixes files
```
pnpm run lint
```