# Lab 7 - Starter

__Name__: Ryan Awal <br>
__Partner__: _None_ <br>

## Check Your Understanding Questions

1. `(Option 1) Within a Github action that runs whenever code is pushed` <br> 
   _Explanation_ : Automated tests should be run via Github Actions upon code push - as it helps catch bugs early, while keeping code quality high and gives immediate feedback that can be fixed without delays.

2. __No__ <br>
   _Explanation_ : E2E tests are meant for testing entire user flows, not individual function outputs. For checking outputs of functions - we can use unit tests instead.

3. The difference between `Navigation mode` and `Snapshot mode` is as follows:
   * `Navigation mode` evaluates the performance of the page from scratch - as it loads up. It captures UX data - how long does the main content of the page take to appear - however, it cannot capture or analyze interactions or changes in content.
   * `Snapshot mode` performs its evaluation on the freeze frame of the current page state. It focuses on static analysis of the HTML, CSS and other assets, without simulating a full page load. It is suited towards checking accessibility issues, SEO and layout.

4. The three improvements we could do to improve the __CSE 110 shop site__ basis its Lighthouse results are:
   * The lighthouse report said that the `<html> element does not have a [lang] attribute`. This poses an accessibility issues as the lang attribute helps screen readers understand language context. The solution is to add language attribute to the root `<html>` tag : `<html lang="en">`
   * The lighthouse report also said that the html " Does not have a `<meta name="viewport">` tag with _width_ or _initial-scale_ No `<meta name="viewport">` tag found". This impacts not only mobile friendliness - but also performance. The solution - a responsive `<meta name="viewport" content="width=device-width, initial-scale=1">` tag can help prevent upto a 300ms delay to user input.
   * The lighthouse report finally also says that " The document does not have a meta description " - which can reduce its visibility in search results. "Meta descriptions may be included in search results to concisely summarize page content". Thus, the solution is to add a descriptive `<meta>` tag in the `<head>` section to improve SEO: `<meta name="description" content="CSE 110 Shop - Your one-stop destination for premium electronics, clothing, and accessories.">`





