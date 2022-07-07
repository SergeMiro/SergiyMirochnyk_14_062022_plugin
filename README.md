# P14-plugin-sergiy-mirochnyk

P14-plugin-sergiy-mirochnyk is a modal library, is wrritten in Javascript. It is a minimal library without any other dependencies, while being performant and straightforward to use, requiring developers to write fewer lines of code than other form libraries.

# Installation

Install P14-plugin-sergiy-mirochnyk with npm
````javascript
npm install p14-plugin-sergiy-mirochnyk
````
# Example
````javascript
import React, { useState } from 'react'
import { Modal } from 'p14-plugin-sergiy-mirochnyk'

export const App = () => {
  const [modalIsOpen, setModalIsOpen] = useState(true);

  return (
    <>
      <h1 style={{ textAlign: 'center' }}>Background</h1>
      <Modal
        show={modalIsOpen}
        setShow={setModalIsOpen}
        title="Success !"
        text="The new employee has been created"
        image={done}
      />
    </>
  );
};
````

## Props

| Name            | Type          | Required | Description                                                              | Default value     |
| --------------- | ------------- | -------- | ------------------------------------------------------------------------ | ----------------- |
| title | `string` | `Required`   | `Modal title`|  `""` |
| width | `string` | `Optinal`  | `Modal width`|  `""` |
| onClose | `function` | `Required`   | `on click : close modal`|  |
| modalContent    | `Required`  | `true`   | Content of the body of the modal                                                     | `{<p></p>}`              |
| footerContent   | `Optional` | `false`  | buttons to add to the footer        | `{<button></button>}`                                                                       |
| isOpen        | `number`     | `Required`  | if isOpen=1 the modal is displayed

              
## Running Tests

To run tests, run the following command

```bash
  npm run test
``` 