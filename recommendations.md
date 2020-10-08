# Conscious Language in your Project: Best Practices and Recommendations

The Conscious Language working group at Red Hat is striving to ensure that Red Hat products, and the upstream projects on which we rely, use welcoming language, free from offensive, othering, or otherwise problematic language.
This includes, but is not limited to, terms with racist, sexist, ableist, or other discriminatory overtones.

To this end, we recommend the following practices in your projects:

## Assessment

In this phase, you will look at your project code, documentation, and web presence looking for words and phrases identified in [our FAQ](https://github.com/conscious-lang/conscious-lang-docs/blob/master/faq.md).
If these assets are stored in Git, we have tools to simplify this process, which we can share with you, or run on your behalf.

This will give you a very high level view of the scope of the work to be done, but more work is needed to figure out the actual level of effort involved in remediation.

We recommend that the assessment phase be a simple count - how many occurrences of the target words/phrases are there in the code and documentation.
For many projects, this phase results in a “nothing to do” verdict and, in itself, is a good data point worth mentioning to your community, and sharing with the Red Hat conscious language team.

The Red Hat Conscious Language group is developing a dashboard that will track progress on the projects we are following.

## Impact survey

Problematic language in your project falls into four major categories, each of which has a very different level of effort needed to address.

1. Words and phrases that appear in documentation, web pages, or code comments, but do not directly relate to keywords, variables, function names, and so on, in the actual code.
These can simply be changed to better alternatives with no functional impact.
2. Words that are in code can sometimes be changed with no functional impact (e.g., local variable names, function names that are only called inside the project code and not accessed externally.)
3. Function names or configuration directives which are exposed externally, such as via an API or a configuration file, require a deprecation plan, so that you do not risk breaking production deployments.
4. And finally there are functional calls into other projects, APIs, services, and so on, which you cannot change until that other project/service changes.
We recommend writing wrapper functions so your code can be “clean”, but still work with third-party code.

Changes in categories 1 and 2 are a great place to judge the community’s appetite for changes in categories 3 and 4, and so we recommend you have early conversations around those changes.

## Remediation

Remediation will be different for every project, but we have some recommendations.

### Radiate Intent

Perhaps the most important thing about remediation is communicating what you’re doing - to your developers, your users, your customers - anybody who has a stake in the change. This is particularly critical with changes in category 3 (above).

If you use tags/labels in your tickets and/or git commits/pull requests, we recommend the use of the tag ‘inclusion’, as recommended in [this blog post](https://medium.com/@sunnydeveloper/squash-inclusion-bugs-982a3e5ee29d). This will allow potential contributors to find these tickets quickly, and will also allow us to identify other projects working on the same issue once the label begins to spread.

### Expect Pushback

Members of your community may object to these changes.
Keep in mind that the goal of these changes is to create a more welcoming community, and respond compassionately to these objections.
We recommend watching Rich Bowen’s presentation [Community Central: Welcoming Nomenclature](https://www.youtube.com/watch?v=hZuFeFuazwo), which addresses common objections to making these changes.

### Clear Deprecation Communication

For changes in categories 3 and 4, clearly communicate the deprecation schedule.
Exact details of this will vary depending on the usage and update patterns of your community.
The focus here is on not breaking production deployments by making changes too quickly.
Leaving several releases between announcing the change, and making it, gives your users an opportunity to become aware that continuing to use old function names, configuration directives, and so on, will cause breakage in future releases.

We define deprecation as a clear period of time during which both the new and old terms work, but using the old term results in a warning (initially) or error message (later on) while not interrupting functionality.

### Wrapper Functions

For changes in category 4 - where you are calling a function in an external library or service that uses words you want to replace - that you write a wrapper function around those functions.
This allows you to fix the problem in your own code, while still calling the problematic function in the external code.
This also gives you a quick path, later on, to discarding the wrapper when the external code gets fixed.

### Test, test, test

Take your time making the changes, and ensure that you’re running all of your tests with every change.
Particularly with changes in categories 3 and 4, there may be far-reaching effects of the changes that you do not anticipate.

## Ongoing vigilance

These changes can be a lot of work, and you want to avoid having to do it twice.
Ongoing vigilance ensures that the issues do not creep back into your project, requiring a second change effort.

### Include language choices in your coding style docs

Tell people what you expect, and enforce it.
Put it in your patch review process so that non-compliant changes are caught before they result in additional technical debt.
Refer to the [Linux kernel coding style guide](https://www.kernel.org/doc/html/v4.10/process/coding-style.html) as an example of this.
This should be in your main style guide, rather than as a separate document, to make it more easily discoverable.

### Mention it in developer onboarding

Tell new contributors that this is what you expect.
Don’t apologize for it.
Have a document that explains why it matters, or point to our document about this.

### Re-run assessment tools regularly

GoTo 1.
Ensure that nothing has crept into your code or documentation by routinely scanning for these terms.
As we update our tooling, you may wish to start scanning for other words and phrases, based on feedback from your community.
Let us know how it’s going!


