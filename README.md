## Deploy React app to gh-pages 

This Action will automate the process of building and depolying react app to gh-pages.

## Action 
Add this action inside your Repository's Actions

```
name: Build and deploy react to gh-pages

on:
  push:
    branches: [ master ]
  pull_request:
    branches: [ master ]

jobs:
  build:

    runs-on: ubuntu-latest
    
    steps:
    - uses: actions/checkout@v2
    - name: Use Node.js ${{ matrix.node-version }}

    - name: Deploy React app to Github pages
      uses: tanwanimohit/deploy-react-to-ghpages@v1.0
```
