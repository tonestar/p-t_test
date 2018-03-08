## Notes

Some considerations
- I've relied on the browser to render most of the dropdown functionality - to make this prettier I would add more control using some form of plugin like Select2 or equivalent. However, leveraging the native browser styles does allow for good accessiblity.
- A more elegant way of handling labels in textfields could have been to use placeholders but that runs into accessiblity issues. Another approach would be to position the label absolutely on top of the form and move it when the user interacts with it but it can be tricky to get the  feel of this interaction spot on.
- This will fall back to HTML5 validation easily enough but some of the JS driven conditional logic will not apply
- This has been tested across the three main OSX browsers of Chrome, Safari, and Firefox. I would also test on iPhones (latest and -1 generation), Android (latest and -1 generation), Chrome PC, Firefox PC, and IE down to IE10 - there is generally under 1% of worldwide users on an IE browser lower than 10 but it depends on your specific client's stats.
- Ideally the JS and Fonts would be served locally - for ease of loading and compactness I have chosen to have these served externally.
- Ideally the JS and CSS would be compressed/minified from seperate files and loaded rather than built in the web page but again, for compact and quick transfer I have chosen to write these directly into the file

My thought process:
I chose JQuery and JQuery validator as I thought these would give the result required in the shortest amount of time with the largest amount of browser support. I also chose JQuery validator as I felt it was far more flexible on a code level than http://www.formvalidator.net/. A quick google gave me this result https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Form_validation which helped me quickly refresh my memory on form validaton.


# [Form validation problem]

We've created this problem to evaluate how developers tackle a real-world problem. If you've been assigned this problem you should spend around **2 hours** working on it. 

## Problem definition

Included is an [index.html] file that contains a form. You must ensure all of the following rules are met before the form is posted to the (in this case imaginary) server:

* `Email` must be a valid email address.
* `Password` must be longer than 8 characters. 
* `Colour` must be selected. 
* At least two `Animal`s must be chosen. 
* If `Tiger` is one of the chosen `Animal`s then `Type of tiger` is required to be a non-empty string. 

## Other requirements

If the form is submitted and an error occurs, the error element's parent should have a CSS `error` class added to it.

```html
<p class="error">
    <label for="field"></label>
    <input id="field" type="text" value="foo">
</p>
```


## The cherry on the cake

Beyond the problem statement, show us the consideration you have given to some or all of the following:

- Documentation
- Accessibility
- Progressive enhancement
- Beautifying ( a hard task on a form I know!)
- Browser support
- Testing
- Tooling

## Submission

Please upload to github and email us a link to your repository

