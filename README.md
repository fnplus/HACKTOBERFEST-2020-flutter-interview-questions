# Flutter Interview Questions with Answers

This repository is a part of [HacktoberFest-an event organised by DigitalOcean](https://hacktoberfest.digitalocean.com/). 
You are requested to create your profile using the above link to be a part of it.

1. What is `Flutter`?

   Flutter is Google's UI toolkit for crafting beautiful, natively compiled applications for mobile, web, and desktop from a single codebase.

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
   
5. What is `Dart`? Why Flutter uses Dart as Programming Language?
   
   Dart is an object-oriented, garbage-collected programming language that you use to develop Flutter apps. It is created by Google. Dart was chosen as the language of Flutter      for the following reason:
   
   i. ***Dart is AOT (Ahead Of Time) compiled*** to fast, predictable, native code, which allows almost all of Flutter to be written in Dart. This makes Flutter fast
   
   ii. ***Dart can also be JIT (Just In Time) compiled*** for exceptionally fast development cycles and game-changing workflow (hotreload).
   
   iii. ***Dart allows Flutter to avoid the need for a separate declarative layout language*** like XML, because Dart’s declarative, programmatic layout is easy to read and visualize. i.e we can do both UI and Buisness Logic using one language only which is ***"DART"***
   
   iv. ***Dart Team + Flutter Team*** As both Dart and Flutter is developed and maintained by Google, hence both Flutter Team and Dart Team work together to solve the problem.  

6. What is the difference between `NetworkImage` and `Image.network` in flutter?

   `NetworkImage` class creates an object the provides an image from the src URL passed to it. It is not a widget and does not output an image to the screen.
   `Image.network` creates a widget that displays an image on the screen. It is just a named constructor on the Image class (a stateful widget). It sets the image property using the NetworkImage . This image property is used finally to display the image.


7. What are `mixins` in dart?

   Mixins are used for a unique kind of inheritance, they allow other classes to inherit it's baked in methods for use, without actually being a child of the parent Mixin class. In simple words, Mixins are our usual normal classes from which we can borrow methods, without extending the class.
   
8. What is `hot reload` in flutter?

   Flutter’s hot reload feature helps you quickly and easily experiment, build UIs, add features, and fix bugs. Hot reload works by injecting updated source code files into the running `Dart Virtual Machine (VM)`. After the VM updates classes with the new versions of fields and functions, the Flutter framework automatically rebuilds the widget tree, allowing you to quickly view the effects of your changes.
	
9. What are the two types of `Streams` available in `Flutter`?
   
   There are two types of Streams available in Flutter which are:
      ..* Single subscription streams
      ..* Broadcast streams
   `Single subscription streams` : It is a popular and commom type of stream. It consist of series of events that are parts of a large whole. The events here have to be delivered in a defined order without even missing a single event.

   `Broadcast streams` : This stream is meant for the individual messages that can be handeled one at a time. Multiple `listener` can listen at a time and it also gives the user the chance to listen after the cancellation of the previous subscription.


10. What is a `Flutter Inspector` ?
   
   `Flutter Inspector` is a tool that helps in visualizing and exploring the widget trees. It also helps in understanding the present layout and rectify the layout issues.


11. Is CI/CD possible in `Flutter`?

    Yes, CI/CD is possible in `Flutter`. There is CI/CD tool dedicated to `Flutter` the name is `CODE MAGIC`. With the help of `CODE MAGIC` we can easily automate the process of CI/CD for flutter apps from single automation.
   
   
12. What’s the difference between `hot reload` and `hot restart`?
    
    Hot reload maintains the app state while updating the UI almost instantaneously whereas Hot restart resets the app state to its initial conditions before updating the UI.


13. What are Null-aware operators in `Flutter` ?    

     Dart offers some handy operators for dealing with values that might be null.

     a.One is the ??= assignment operator, which assigns a value to a variable only if that variable is currently null<br>
     b.Another null-aware operator is ??, which returns the expression on its left unless that expression’s value is null, in which case it evaluates and returns the expression        on its right

14. What is use of `Navigation.push` and `Navigation.pop` function? 
   
    The `push` method is used to add a route to the stack of routes managed by the navigator. The `pop` method is used to remove the current route from the stack of routes managed by the navigator.


15. What is an `App state`? 
    
    State means that is not ephemeral, that you want to share across many parts of your app, and that you want to keep between user sessions, is what we call application state (sometimes also called shared state).

      ***Examples of application state:***
   * User preferences
   * Login info
   * Notifications in a social networking app
   * The shopping cart in an e-commerce app
   * Read/unread state of articles in a news app

16. What are the `different build modes` in Flutter?

   * The Flutter tooling supports three modes when compiling your app, and a headless mode for testing.
   * You choose a compilation mode depending on where you are in the development cycle.
  
   * The modes are:
     * Debug
     * Profile
     * Release

17. What is the difference between *`main()`* and *`runApp()`* functions in Flutter? 

   * `main ()` function came from Java-like languages so it's `where all program started,` without it, you can't write any program on Flutter even without UI.
   * `runApp()` function should return Widget that would be attached to the screen as a root of the Widget Tree that will be rendered.

18. What is ***ScopedModel/BLoC Pattern?***
    
    `ScopedModel` and `BLoC (Business Logic Components)` are common Flutter app architecture patterns to help separate business logic from UI code and using fewer Stateful Widgets.

    * `Scoped Model` is a third-party package that is not included into Flutter framework. It's a set of utilities that allow you to easily pass a data Model from a parent Widget down to its descendants. In addition, it also rebuilds all of the children that use the model when the model is updated. This library was originally extracted from the Fuchsia codebase.
   
    * `BLoC` stands for Business Logic Components. It helps in managing state and make access to data from a central place in your project. The gist of BLoC is that everything in the app should be represented as stream of events: widgets submit events; other widgets will respond. BLoC sits in the middle, managing the conversation.

19. How to avoid widget remount while working with Bottom navigation tabs?

    The effective way to avoid the no of widget rebuilds while working with multiple Widgets as interfaces of a app that uses Bottom Navigation Tabs as it's stratergy it to utilize IndexedStack that will increase the app performace by 2x and reduces the unnecessary widget rebuilds on tab changes.

20. How do you reduce widget rebuild?

   You rebuild widgets when the state changes. This is normal and desirable, because it allows the user to see the state changes reflected in the UI. However, rebuilding parts of the UI that don't need to change is wasteful.

   There are several things you can do to reduce unnecessary widget rebuilding.

   * The first is to refactor a large widget tree into smaller individual widgets, each with its own `build` method.
   * Whenever possible, use the `const` constructor, because this will tell Flutter that it doesn't need to rebuild the widget.
   * Keep the subtree of a stateful widget as small as possible. If a stateful widget needs to have a widget subtree under it, create a custom widget for the stateful widget and give it a `child` parameter.
   
21. What is `BuildContext` and how is it useful?

   BuildContext is actually the widget's element in the Element tree — so every widget has its own BuildContext.
   You usually use BuildContext to get a reference to the theme or to another widget. For example, if you want to show a material dialog, you need a reference to the scaffold. You can get it with Scaffold.of(context), where context is the build context. of() searches up the tree until it finds the nearest scaffold.

22. What is `setState()` ?
   
  setState notifies the framework that the internal state of an object has changed in a way that might impact the user interface in this subtree, which causes the framework to schedule a build for this State object. If we just change the state directly without calling setState, the framework might not schedule a build and the user interface for this subtree might not be updated to reflect the new state.
  It is recommended that the setState method only be used to wrap the actual changes to the state, not any computation that might be associated with the change.
  
23. Explain why the `Arrow operator` is used in Flutter?

  The Arrow operator is the only one line of code and is a shorthand in Dart, which can we used to write one-line functions.

24. What is the purpose of a `SafeArea`?

   `SafeArea` is basically a glorified Padding widget. If you wrap another widget with `SafeArea` , it adds any necessary padding needed to keep your widget from being blocked by the system status bar, notches, holes, rounded corners and other "creative" features by manufactures.

25. What is the difference between `WidgetsApp` and `MaterialApp`?
   
   `WidgetsApp` provides basic navigation. Together with the `widgets` library, it includes many of the foundational widgets that Flutter uses.
   `MaterialApp` and the corresponding `material` library is a layer built on top of `WidgetsApp` and the widgets library. It implements Material Design, which gives the app a unified look and feel on any platform or device. The `material` library has many additional widgets that come with it.
   You certainly aren’t required to use `MaterialApp` in your project. You can use `CupertinoApp` to make iOS users feel at home, or you can even build your own set of custom widgets to fit your brand.

26. Can you nest a `Scaffold`? Why or why not?

   Yes, you can absolutely nest a `Scaffold`. That’s the beauty of Flutter. You control the entire UI.
   `Scaffold` is just a widget, so you can put it anywhere a widget might go. By nesting a `Scaffold`, you can layer drawers, snack bars and bottom sheets.

27. When is it appropriate to use packages, plugins or third-party dependencies?

   Packages and plugins are great for saving you time and work. There’s no need to solve a complex problem yourself when someone else has done it already, especially if the solution is highly rated.
   On the other hand, there’s also a danger of being too reliant on third party packages. They can break, have bugs or even be abandoned. When you need to switch to a new package down the road, you might have to make huge changes to your code.
   That’s why it’s important to isolate packages from your core business logic. You can do that by creating an abstract Dart class that acts as an interface for the package. Once you’ve set up that kind of architecture, all you have to do to switch packages is to rewrite the concrete wrapper class that implements your interface.

28. What types of tests can you perform?

   There are three main kinds of tests: unit tests, widget tests and integration tests. Unit tests are all about checking the validity of your business logic. Widget tests are for making sure UI widgets have the components that you expect them to. Integration tests check that your app is working as a whole.
   One additional type of test that is not as well known is a golden test. In a golden test, you have an image of a widget or screen and check to see that the actual widget matches it.

29. How do you talk to native code from within a Flutter app?

   One type of platform channel is a method channel. Data is serialized on the Dart side and then sent to the native side. You can write native code to interact with the platform before sending a serialized message back. That message might be written in Java or Kotlin on Android or Objective-C or Swift on iOS.
   The second type of platform channel is the event channel, which you use to send a stream of data from the native platform back to Flutter. This is useful for monitoring sensor data.
   
30. Why does the first Flutter app build take so long?

   When you build the Flutter app the first time, it will take a longer time. It is because the Flutter builds the device-specific APK or IPA file. Thus, the Gradle and Xcode are used to build the file, taking a long time.
   
31. What is the purpose of @override used in Flutter?

   @override points out that the function is also defined in an ancestor class, but is being redefined to do something else in the current class. It's also used to annotate the implementation of an abstract method. It is optional to use but recommended as it improves readability.
   
31. What are the different build modes in Flutter?

   The Flutter tooling supports three modes when compiling your app, and a headless mode for testing. You choose a compilation mode depending on where you are in the development cycle.The modes are: 
   - Debug 
   - Profile 
   - Release
   

   

   



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
