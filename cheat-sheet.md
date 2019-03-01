> Note: This is a copy of the original GitHub Craftwork cheat sheet

# GitHub Craftwork

Welcome to the Craftwork cheat sheet! This page has everything you need to make it through the Craftwork workshop. If you don’t see the next step, or you have questions that aren’t answered by the FAQ below, don’t be afraid to raise your hand and ask us!

# Part 1: Hello World

Begin by making a sandbox repository, to keep everything nice and contained. https://github.com/new

Next, we begin by remixing an existing app boilerplate on Glitch: https://glitch.com/edit/#!/remix/craftwork

Follow the instructions in the Glitch app to get everything set up. Don’t forget to upload an avatar, or it uses yours and it might be confusing.

Can’t find the App dashboard? It’s here: https://github.com/settings/apps

Once you’re done, try creating an issue in your sandbox repository. Did you get a response that reads “Hello world!”? Awesome! If not, raise your hand, and someone will come by to help you troubleshoot.

# Part 2: The Twist

Now, let’s change our code up. Instead of replying to new issues, let’s triage them. The goal is to build an app that will look at incoming issues, and classify them as “bug reports”, “feature requests”, or “questions” automatically for us! Let’s use some fun NLP for that.

What we will need to do is this:

Grab the title of the issue
Pass the title to a text classification API—recast.ai
Determine whether the title is a command, a request, or a question
Add labels to the issue dependingon on how we classified the text
What was the URL for API we’re using? It’s https://recast.ai. A more detailed explanation on building a Recast bot can be found on the blog.github.com.

Remember to add the recastai npm package to your Glitch App. You can also learn how to add npm packages in Glitch from the Glitch Forum link.

Want the step-by-step code for index.js? https://gist.github.com/DEGoodmanWilson/90a209a16d7fe700f60c5d25fd0a95c4

Here is the complete code for index.js, if you get lost adding the code to your project: https://gist.github.com/DEGoodmanWilson/9be15fb522ae538509d580c48f24d4a8

Finally, test it! Open some sample issues in the sandbox repo, and watch how the app tags each of them. It’s not perfect, but it should serve as an inspiration to go further!
