# Flutter Interview `Questions` with `Answers`

This repository is a part of [HacktoberFest-an event organised by DigitalOcean](https://hacktoberfest.digitalocean.com/). 
You are requested to create your profile using the above link to be a part of it.

1. What is `Flutter`?

   `Flutter is Google's UI toolkit for crafting beautiful, natively compiled applications for mobile, web, and desktop from a single codebase.`

2. What are the `different types of widgets in Flutter`?

   Two types of widgets present in the Flutter are stateless and stateful.

   The stateless widgets don’t store any values which will change in the future. 
   The stateless widgets don’t store any state. Icon, text widgets are some examples of stateless widgets.

   The stateful widgets have a state object to keep track of all the changes and updates happening in the UI. 
   These widgets are immutable but the state object is used to keep track of the changes. 
   Checkbox and image are some of the examples of stateful widgets.

3. Difference b/w `Stateful` widget and `Stateless` widget.
   
   Stateless widgets cannot change their state during the runtime of the app, 
   which means the widgets cannot be redrawn while the app is in action. 

   Stateful Widgets are the ones that change its properties during run-time. 
   They are dynamic i.e., they are mutable and can be drawn multiple times within its lifetime. 
   

4. What is the use of `pubspec.yaml` file in `Flutter`?

   The pubspec. yaml file is the most important file in any Flutter project. 
   It is the place where you provide all the required dependencies of your Flutter project.
   
5. What is Dart? Why Flutter uses Dart as Programming Language?
   Dart is an object-oriented, garbage-collected programming language that you use to develop Flutter apps. It is created by Google. Dart was chosen as the language of Flutter      for the following reason:
   
   i. ***Dart is AOT (Ahead Of Time) compiled*** to fast, predictable, native code, which allows almost all of Flutter to be written in Dart. This makes Flutter fast
   
   ii. ***Dart can also be JIT (Just In Time) compiled*** for exceptionally fast development cycles and game-changing workflow (hotreload).
   
   iii. ***Dart allows Flutter to avoid the need for a separate declarative layout language*** like XML, because Dart’s declarative, programmatic layout is easy to read and visualize. i.e we can do both UI and Buisness Logic using one language only which is ***"DART"***
   
   iv. ***Dart Team + Flutter Team*** As both Dart and Flutter is developed and maintained by Google, hence both Flutter Team and Dart Team work together to solve the problem.  

6. What is the difference between `NetworkImage` and `Image.network` in flutter?

   `NetworkImage` class creates an object the provides an image from the src URL passed to it. It is not a widget and does not output an image to the screen.
   `Image.network` creates a widget that displays an image on the screen. It is just a named constructor on the Image class (a stateful widget). It sets the image property using the NetworkImage . This image property is used finally to display the image.


7. What are mixins in dart?

   Mixins are used for a unique kind of inheritance, they allow other classes to inherit it's baked in methods for use, without actually being a child of the parent Mixin class. In simple words, Mixins are our usual normal classes from which we can borrow methods, without extending the class.
   
8. What is hot reload in flutter?

   Flutter’s hot reload feature helps you quickly and easily experiment, build UIs, add features, and fix bugs. Hot reload works by injecting updated source code files into the running `Dart Virtual Machine (VM)`. After the VM updates classes with the new versions of fields and functions, the Flutter framework automatically rebuilds the widget tree, allowing you to quickly view the effects of your changes.
	




8. What are the two types of `Streams` available in `Flutter`?
   
   There are two types of Streams available in Flutter which are:
      ..* Single subscription streams
      ..* Broadcast streams
   `Single subscription streams` : It is a popular and commom type of stream. It consist of series of events that are parts of a large whole. The events here have to be delivered in a defined order without even missing a single event.

   `Broadcast streams` : This stream is meant for the individual messages that can be handeled one at a time. Multiple `listener` can listen at a time and it also gives the user the chance to listen after the cancellation of the previous subscription.


9. What is a `Flutter Inspector` ?
   
   `Flutter Inspector` is a tool that helps in visualizing and exploring the widget trees. It also helps in understanding the present layout and rectify the layout issues.


10. Is CI/CD possible in `Flutter`?

   Yes, CI/CD is possible in `Flutter`. There is CI/CD tool dedicated to `Flutter` the name is `CODE MAGIC`. With the help of `CODE MAGIC` we can easily automate the process of CI/CD for flutter apps from single automation.

12. What are Null-aware operators in `Flutter` ?    

     Dart offers some handy operators for dealing with values that might be null.

     a.One is the ??= assignment operator, which assigns a value to a variable only if that variable is currently null<br>
     b.Another null-aware operator is ??, which returns the expression on its left unless that expression’s value is null, in which case it evaluates and returns the expression        on its right

13. What is use of `Navigation.push` and `Navigation.pop` function? 
   
    The `push` method is used to add a route to the stack of routes managed by the navigator. The `pop` method is used to remove the current route from the stack of routes managed by the navigator.
    
 
 14. What’s the difference between `hot reload` and `hot restart`?
     Hot reload maintains the app state while updating the UI almost instantaneously whereas Hot restart resets the app state to its initial conditions before updating the UI.




## Contributors


[![](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/images/0)](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/links/0)[![](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/images/1)](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/links/1)[![](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/images/2)](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/links/2)[![](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/images/3)](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/links/3)[![](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/images/4)](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/links/4)[![](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/images/5)](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/links/5)[![](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/images/6)](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/links/6)[![](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/images/7)](https://sourcerer.io/fame/xlogix/fnplus/flutter-interview-questions/links/7)

## Contributing

1. Have a look at open issues. Pick an unassigned issue. 
2. You can also create new issues (If you add a question or want answer to a particular question ).
3. **Make sure you are assigned for the issue.**
4. Fork the repo!
5. Clone the forked repository to local system.
6. Create your feature branch: `git checkout -b my-question-answer`
7. Be sure to not include any compiled binaries in the patch.
8. Commit your changes: `git commit -am 'Add some question/answer'`.
   Go through [Commit Messages guidelines](CONTRIBUTING.md#write-good-commit-messages)
9. Push to the branch: `git push origin my-question-answer`
While sending a PR make sure you follow one issue per PR rule.
10. Submit a pull request :smile:

## Notes:

Only project maintainers should merge a PR.
Other members can add their reviews to a PR but the merging should be done by only a project maintainer.

## Authors:

* [Abhishek Kumar](https://github.com/imabhishekkumar)
* [Abhishek Uniyal](https://github.com/xlogix)
