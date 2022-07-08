# P14-plugin-mirochnyk-s

p14-plugin-mirochnyk-s is a modal library, is wrritten in Javascript. It is a minimal library without any other dependencies, while being performant and straightforward to use, requiring developers to write fewer lines of code than other form libraries.


# Installation

Install p14-plugin-mirochnyk-s with npm

```javascript
npm install p14-plugin-mirochnyk-s
```

# Example

```javascript
import React, { useState } from 'react';
import { Modal } from 'p14-plugin-mirochnyk-s';

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
```

## Running Tests

To run tests, run the following command

```bash
  npm run test
```
