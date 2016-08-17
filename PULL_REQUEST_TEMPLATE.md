Added event listeners, hid article excess (and showed again), and category/author sorting selectors to blog.

Today, Megan and Lee paired together. It took about 3 hours.

Reflect and summarize on your process for each TODO item :

1. Lee drove. The first TODO was designed to hide all of the existing articles while fading in ONLY the articles that 
has the same category as the one we selected. We also had it set up that if the selectors aren't picking anything, 
it will show all articles.

2. Lee drove. Second TODO was to create a filter selector for authors in addition to the category one above. Was almost the
same code. We also set it up so that if one selector is used, the other is reset.

3. First thing we did when Megan started driving was to add in our new script to our html file. We hid all of the tab-content
sections. We wrestled with making the fade-in work properly, as well as on page load. We wanted to be able to load the page
and simulate a click event for when the home tab is clicked so that it auto-loads on page load.

4. Finally, we worked on revealing the entire article beyond the two lines. We spent some time trying to figure out how to
traverse the DOM to get to a sibling element. We realized we could just target the link a tag, go above to the parent, and 
use the * selector to show everything. At that point, there's nothing to hide, so targeting doesn't need to be so specific.

Key take-aways/learnings:
- Delegation doesn't work on event.target, so we should always use 'this'. <---Worth examining what outlier scenarios 
event.target should be used on.
- Traversal of the DOM and using specific CSS-like DOM traversal methods (ie parent(), (siblings(), etc.)
- Simulating a click can be done without a click. Meaning, you can have an event happen without a click even if it requires
a click.
- If you name your data the same as an id, you can use that as a selector.

Checklist (before submitting, fill in each set of square brackets with an 'x')

[X] We have titled the Pull Request similar to our branch name (ex: 'brian-rick').
[X] This PR includes commits from both myself and my partner; e.g. We followed good pair programming practices by switching driver/navigator roles.
[X] There is no extraneous, unrelated code included in this PR.
[X] We have summarized our TODO: process above.
