# 分号(Semicolons)

## **Yup.**

  eslint rules: [`semi`](http://eslint.org/docs/rules/semi.html).

  ```javascript
  // bad
  (function () {
    const name = 'Skywalker'
    return name
  })()

  // good
  (() => {
    const name = 'Skywalker';
    return name;
  })();

  // good (guards against the function becoming an argument when two files with IIFEs are concatenated)
  ;(() => {
    const name = 'Skywalker';
    return name;
  })();
  ```

  [了解更多](http://stackoverflow.com/questions/7365172/semicolon##before##self##invoking##function/7365214%237365214)。

