# asciidoc-javascript-validator
Validate JavaScript code in AsciiDoc files by linting, executing and testing assertions.

I'm working on a long document, formatted with AsciiDoc, that includes JavaScript code examples.
This repo contains the tool I'm building and using to help me validate those examples.

The tool validates that the code runs, and also validates assertions that are unobtrusively
included in the code int the form of comments. The comment `// => null`, for example asserts
that the expression that preceeds the comment evaluates to null.

I'm now working to run eslint over the code as well.

Note that this is not a general-purpose tool for validating code in technical documents.
It is specific to JavaScript code in AsciiDoc, and is therefore only of interest to
writers using the same toolchain as I am.
