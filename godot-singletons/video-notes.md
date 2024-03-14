# Video Notes: Godot Singletons

This video was more controversial than I anticipated. In hindsight, I should have picked a better example for the Autoload. I tried to find a very approachable example, but simplified to the point where 'Weather Manager' probably should not have been a node at all.

In a nutshell, Singletons are a fairly controversial design pattern, and lots of developers (especially outside of the gamedev space), absolutely refuse to use them. And for good reason too! Singletons are difficult to test, break encapsulation, suffer from the same issues as globals, and circumvent other useful patterns like dependency injection. With that said, they do have a place in gamedev, and I don't regret covering them!

## Corrections

At the risk of misrepresenting the feedback I received, here is a paraphrased list of complaints, for your perusal: 
 - Autoloads in Godot are not *technically* singletons, since there is nothing preventing more instances from being created
 - At the end of the video, I could have moved the shared state into a resource, rather than creating a scene
 - The singleton example I selected was bad, for various reasons

Happy coding!