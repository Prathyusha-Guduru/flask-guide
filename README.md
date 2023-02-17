# flask-guide

### Pre-requisities

- [First-class functions](https://youtu.be/kr0mpwqttM0)

  - a programming language is said to have first class functions if it treats functions as first class citizens
  - First-class citizens/objects - entities which support all the operations generally avaiable to other entities, eg : passing and returning as arguments
    <br/><br/>

- [Closures](https://youtu.be/swU3c34d2NQ)

  ```
  def outer_function():
        m = "Hi"
        def inner_function():
            print(m)
    outer_function()
  ```

  Output of the above code block is none because inner function is returned but not executed. To be able to execute this, we need to

  ```
  new_m_function = outer_function()
  new_m_function
  ```

  The above code block will now print "Hi" in the console. Innter functions which exhibit this behaviour i.e ability to access variables in the local scope that it was created, even after the outer function has finished executing are known as closures. Hence here, inner_function() is a closure.

  <br/><br/>

- ## [Decorators](https://youtu.be/FsAPt_9Bf3U)
