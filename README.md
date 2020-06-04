# react-modal-overlay

### Accessible modal overlay component for React JS
[![NPM](https://img.shields.io/npm/v/react-modal-overlay.svg)](https://www.npmjs.com/package/react-modal-overlay) [![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com) [![Build Status](https://travis-ci.org/akmamun/react-modal-overlay.svg?branch=master)](https://travis-ci.org/akmamun/react-modal-overlay)

## Install

```bash
npm install --save react-modal-overlay
```

## Usage

```jsx
import React, { Component } from "react";
import { Modal } from 'react-modal-overlay'
import 'react-modal-overlay/dist/index.css'

export default class ExampleModal extends Component {
  state = {
    showModal: false
  }

  toggleModal = () => {
    this.setState({
      showModal: !this.state.showModal
    })
  }

  render() {
    return (
      <div>
        <button onClick={this.toggleModal}>Click Modal!</button>
        <Modal show={this.state.showModal} closeModal={this.toggleModal}>
          <h4> here is modal data </h4>
        </Modal>
      </div>
    )
  }
}
```

## Demos
- [Minimal example](https://codesandbox.io/s/react-modal-overlay-wybon) 
## License

MIT © [akmamun](https://github.com/akmamun)
