# React Hubspot Submissions

A Custom React hooks for interacting with Hubspot Submissions API.
Works with Create React App, Next.js, Gatsby and other platforms.

## Installation

```
npm install --save hubspot-submissions
```

or

```
yarn add hubspot-submissions
```

## Usage

```jsx
import { useForm } from "hubspot-submissions";

export default () => {
  const { data, isLoading, isError, handleSubmit } = useForm({
    portalId: "6168888",
    formId: "40faef1c-e68b-4a20-8444-f7079462f0cc",
  });

  return (
    <form onSubmit={handleSubmit}>
      <input name="email" type="text" placeholder="email" />
      ...
      <button type="submit">Submit!</button>
    </form>
  );
};
```
