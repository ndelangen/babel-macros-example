# babel-macros-example

This is a simple example of a [`babel-macros`][babel-macros] macro.

You'll notice that the `input.js` file is importing the `./greeting.macro.js` file
Then the imported identifiers are used throughout the code. The macro itself
is about as simple as you can get with a `babel-macros` macro. It accepts the
references to those imports and replaces the references with string literals.
Take a look at the `output.js` file to see what the result is. Now mess around
with it a bit to see what you can do with this thing!

Hopefully this helps you get started trying out writing a macro!

## Tips

Writing a macro is similar to writing a babel-plugin except you give up a little
power in favor of a simpler setup for you and the user of your macro (maybe also
you). Because it's so similar to writing a babel-plugin, it could be really
helpful to learn how to write babel-plugins and using ASTs. Here are some
resources for that:

- [babel-plugin-handbook][babel-plugin-handbook]
- [Writing custom Babel and ESLint plugins with ASTs][asts-talk]
- [Code Transformation and Linting with Abstract Syntax Trees][fem-asts]

From there, you may also want to reference the [babel-macros docs][babel-macros-docs]

Good luck!

[babel-macros]: https://github.com/kentcdodds/babel-macros
[babel-plugin-handbook]: https://github.com/thejameskyle/babel-handbook/blob/master/translations/en/plugin-handbook.md
[fem-asts]: https://frontendmasters.com/courses/linting-asts/
[asts-talk]: https://www.youtube.com/watch?v=VBscbcm2Mok&index=1&list=PLV5CVI1eNcJgNqzNwcs4UKrlJdhfDjshf&t=192s
[babel-macros-docs]: https://github.com/kentcdodds/babel-macros/blob/master/other/docs/author.md
