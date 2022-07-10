# p14-plugin-miro

p14-plugin-miro is a modal library, is wrritten in Javascript. It is a minimal library without any other dependencies, while being performant and straightforward to use, requiring developers to write fewer lines of code than other form libraries.


# Installation

Install p14-plugin-miro with npm

```javascript
npm install p14-plugin-miro
```

# Example

```javascript
import React, { useState } from 'react'
import 'ReactModalFz/dist/index.css'
import { Modal } from 'p14-plugin-miro'

const App = () => {
const [isOpen, setIsOpen] = useState(0)

return (
      <Modal
         isOpen={isOpen}
         onClose={setIsOpen}
         title='Modal title'
         width='600px'
         modalContent={<p>Modal content</p>}
         footerContent={
            <>
               <button className='btn-modal'>ok</button>
               <button className='btn-modal'
                  onClick={() => setIsOpen(isOpen ? 0 : 1)} >
                  close
               </button>
            </>
         }
      />
)}
```

## Running Tests

To run tests, run the following command

```bash
  npm run test
```
