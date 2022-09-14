# custom-hooks

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- Use the different custom hooks on their projects with reactJS

## My process

### Built with

- Custom Hooks
- JavaScript
- ReactJS

### What I learned

This respository is focus on have a place where can add all the custom hooks that i use in different projects is available to everyone that
want tu use them.

```js proud-of-this:
    import { useState } from "react";

    export const useForm = ( initialForm = {}) => {

    const [formState, setFormState] = useState( initialForm );

    const onInputChange = ({ target }) => {
        const { name, value } = target
        setFormState({
            ...formState,
            [ name ] : value,
        })
    }

    const onResetForm = () => {
        setFormState(initialForm)
    } 

    return {
        ...formState,
        formState,
        onInputChange,
        onResetForm,
    }
}
```

## Author

- Github - [Omar Ascanio](https://github.com/Omared250)
- Frontend Mentor - [@omared250](https://www.frontendmentor.io/profile/Omared250)
