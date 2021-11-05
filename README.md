# Exception error to action protocol 

Exception error to action protocol in typescript.


```typescript

function myError() {
    throw MicroServiceError('Error foobar', 'error-foobar')
}

try {
  myError()
} catch (err) {
  const msError as MicroServiceError;
  console.log(msError.getData())
  /*
    output
    {
      message: 'Error foobar',
      type: 'error-foobar'
    }
  */
}
```
