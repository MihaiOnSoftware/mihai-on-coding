## Roles

The two roles listed above, *driver* and *navigator* serve different purposes. It's often not clear who does what, keeping the guidelines here in mind can be helpful.

### *Driver*

This is the clearest role, at least in part, because it's the person at the keyboard. The *driver* is responsible for the implementation. They keep their focus on what is happening right now and interpret what the *navigator* is saying. It's best if the *driver* doesn't focus too much on the broader design. Instead they should focus on making sure the work they are doing right now is high quality and doesn't contain errors. For example while writing a method as directed by the *navigator*, the *driver* would focus on:

* extracting variables
* extracting private methods
* variable, method, and class names
* other local refactoring and improvements.

### *Navigator*

This role focuses on the broader scope of the *problem*. Generally the *navigator* will set the direction the code should go in. For example they might say something like "We need to add a private method to this class, something like `sanitize_svgs` which would take in an `svg` and return the sanitized verizon by calling out to the `SvgSanitizer`". The *driver* will then take this and put it into code, modifying it to keep the code clean and error free. The *navigator* is also responsible to keeping an eye out for any errors, typos, or refactoring opportunities that crop up and the *driver* misses. Though this is not their primary role it's still important.

The *navigator* should try to keep from grabbing the keyboard, even when the solution seems clear. If a solution can't be communicated clearly enough to the *driver* for implementation, it might not be all that clear of a solution. 

### Dialogue

It's important to note that the *driver* isn't just implementing what the *navigator* says, they are part of a dialogue. The idea here is that the *driver* brings in the "low level" perspective from the code that's in front of them and what will actually work here, the *navigator* brings in a more bird's eye view and tries to imagine how what is being written now will fit in with the greater design. By switching roles with some frequency, the *pair* can ensure that they have a good handle of both perspectives. 
