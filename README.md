# oj-parent
Oddjob Maven Parent

In addition to providing shared properties and defining common dependency versions this 
parent provides the following.

- A logback file override in the plugin definition of the surefire tests that ensures only
  warnings are written to the console, and everything else to a file. This allows tests that assert 
  against console output to still work in Maven. Projects that include the arooa tests jar will get a definition
  automatically.