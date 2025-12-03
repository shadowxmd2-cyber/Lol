# Queen Asha MD MULTIDEVICE WHATSAPP BOT 🥳
<div align="center">

 [![Typing SVG](https://readme-typing-svg.herokuapp.com?font=&pause=1000&color=FFF84CFA&multiline=true&random=true&width=435&lines=Queen+Mini+By+KAVIDU++%26+Ishan+)](https://git.io/typing-svg)
 <img src="https://i.imgur.com/dBaSKWF.gif" height="90" width="100%">


# WORKFLOW CODE 👨‍💻
```
name: Node.js CI

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main

jobs:
  build:

    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [20.x]

    steps:
    - name: Checkout repository
      uses: actions/checkout@v3

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: ${{ matrix.node-version }}

    - name: Install dependencies
      run: npm install

    - name: Start application
      run: npm start

