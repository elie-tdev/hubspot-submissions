# React Hubspot Submissions

A Custom React hooks for interacting with Hubspot Submissions API


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
import { useForm } from 'hubspot-submissions'

export default () => {
  const { data, isLoading, isError, handleSubmit } = useForm({
    portalId: '<PORTAL_ID>',
    formId: '<FORM_ID>'
  })

  return (
    <form onSubmit={handleSubmit}>
      <input name="email" type="text" placeholder="email" />
    </form>
  )
}
```
