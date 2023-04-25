
# A js-like setTimeout function

This library exposes a setTimeout function to the global namespace.

# How to use

The timeout delay is specified by passing a std::chrono::duration as the second argument:

```c++
using namespace std::chrono_literals;

setTimeout([] {
    // code ...
}, 5s); // 5 seconds delay
```

setTimeout is also able to pass parameters to the function to be executed:

```c++
using namespace std::chrono_literals;

setTimeout([](int n) {
    // do something with n
}, 5s);
```
