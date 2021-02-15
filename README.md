# Github Actions Common Lisp Rove Tests

Runs Common Lisp tests using Rove library


Example of use (see [alangalvino/incognia-wrapper](https://github.com/alangalvino/incognia-wrapper)):

```
on: [push]

jobs:
  test:
    runs-on: ubuntu-latest
    name: A job to run Common Lisp tests
    steps:
    - name: Checkout
      uses: actions/checkout@v2
    - name: Install libyaml-dev
      run: sudo apt-get install libyaml-dev
    - name: Run tests (Common Lisp Rove)
      uses: alangalvino/github-actions-cl-rove@v0.0.2
```
