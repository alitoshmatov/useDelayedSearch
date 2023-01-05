# useDelayedSearch

> You can use this react hook to get delayed value of string input, it helps to get final string after typing stops. You can adjust delayed time by passing time in milliseconds to useDelayedSearch hook.

![Usage of useDelayedSearch hook](https://media.giphy.com/media/vmuZXtyhqVXNwvXbA1/giphy.gif)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Installation

To install and set up the library, run:

```sh
npm install -S use-delayed-search
```

Or if you prefer using Yarn:

```sh
yarn add --dev use-delayed-search
```
## How to use

```jsx
  const Component = () => {
    const [value, delayedValue, setValue] = useDelayedSearch(1000);

    return (
      <>
        <input value={value} onChange={(e) => setValue(e.target.value)} />
        <p>Immediate value: {value}</p>
        <p>Delayed value: {delayedValue}</p>
      </>
    );
  };
```
