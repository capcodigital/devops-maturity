[home](../README.md)
# [Test Automation](README.md) - Usability Testing


Usability testing often comes in two forms:

1. Testing features/products with small user groups in person to see how a newly introduced audience reacts to changes.
1. Accessibility testing, your end user might experience from certain limitations that don’t allow them to access information as easy as others.


For this topic, we will be zooming in more on Accessibility testing as this is something you can run automated tests against.

Web accessibility is all about making sites and applications that everyone can use, especially people with disabilities. With a rather large list of competing priorities when building for the web, from accessibility to performance to security, it makes sense to automate parts of the process. Manual testing is a necessity for accessibility, however, a certain amount of the effort can and should be spent on automation, freeing up human resources for more complex or nuanced tasks.

Automated testing is a great way to start weaving accessibility into your website, with the goal of shifting left more and more towards the UX and discovery process. Automated testing can’t catch everything, but it’s a valuable way to address easy wins and prevent basic fails. Build accessibility into your UI code, document features for teams, and ideally, prevent regressions in quality from deploying to production.

For accessibility testing the focus is more put on unit and integration tests. A unit test typically covers underlying APIs that plumb accessibility information or interactions to the right place. You should test APIs in isolation, calling their methods with fake data, called “inputs”. You can then assert these method calls modify the application or its state in an expected way.

An example of such a test:

```
it('should pass aria-label to the inner button', inject(function() {
    var template = '&lt;custom-button label="Squishy Face"&gt;&lt;/custom-button&gt;';
    var compiledElement = make(template);
    expect(compiledElement.find('button').attr('aria-label')).toEqual('Squishy Face');
}));
```

It’s debatable whether a unit test should assert actual focus in the DOM, such as document.activeElement being an expected element. Unit testing tools frequently fail at the task, and you’ll end up chasing down bugs related to your test harness instead of writing useful test cases.

You can try using [Simulant](https://www.npmjs.com/package/simulant), so long as keyboard focus is tested within a single unit, perhaps within an isolated component. In that case, go for it (and let me know which tools you end up using)! However, keyboard focus is often better tested in the integration realm, both because of ease in tooling and because a user’s focus frequently moves between multiple components (thus stepping outside the bounds of a single code unit).

Instead of unit testing interactions and expecting a focused element, you can write unit tests that call related API methods with static inputs, such as state variables or HTML fragments. Then you can assert those methods were called and the state changed appropriately.


Read more here:

[Writing Automated Tests for Accessibility](https://www.deque.com/blog/writing-automated-tests-accessibility/)
[Evaluating Web Accessibility Overview](https://www.w3.org/WAI/test-evaluate/)
