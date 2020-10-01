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
   

5. What is the difference between NetworkImage and Image.network in flutter?

   NetworkImage class creates an object the provides an image from the src URL passed to it. It is not a widget and does not output an image to the screen.
   Image.network creates a widget that displays an image on the screen. It is just a named constructor on the Image class (a stateful widget). It sets the image property using the NetworkImage . This image property is used finally to display the image.


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
