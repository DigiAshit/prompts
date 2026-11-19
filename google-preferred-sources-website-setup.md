# Google Preferred Sources: Complete Website Setup Guide

Google Preferred Sources lets people choose websites they want to see
more often in eligible Google Search experiences. Website owners can
make it easier for visitors to select their site by adding Google's
official Preferred Sources button.

> **Important:** Adding the button does not guarantee higher rankings or
> placement in Google Search, AI Overviews or AI Mode. Visitors must
> choose the site themselves, and Google decides when content is
> eligible and relevant to show.

## 1. Check your website

Before implementing the button:

1.  Open [Google Preferred
    Sources](https://www.google.com/preferences/source).
2.  Search for your website or publication.
3.  Check whether Google recognises it as a source that can be selected.

A domain or subdomain may be selectable. A subdirectory (for example,
`example.com/blog`) is not independently selectable as a separate
source.

For visibility in AI Overviews and AI Mode, your site must also meet
Google's eligibility requirements for Search generative AI features.
Adding the button alone does not make a site eligible.

## 2. Add Google's JavaScript library

Add this script to the `<head>` section of your website:

``` html
<script async src="https://news.google.com/swg/js/v1/publisher.js"></script>
```

Add the script only once per page, even if the button appears in more
than one location.

## 3. Add the Preferred Sources button

Place this element inside the `<body>` wherever you want the button to
appear:

``` html
<div google-add-preferred-source-btn></div>
```

Google's library will render the button.

Good placement options include:

-   Your website header or navigation area.
-   A blog sidebar.
-   The end of an article.
-   Your website footer.

Choose a visible location without making the button intrusive.

## 4. Optional button customisation

You can set a theme:

**Light theme**

``` html
<div
  google-add-preferred-source-btn
  data-theme="light">
</div>
```

**Dark theme**

``` html
<div
  google-add-preferred-source-btn
  data-theme="dark">
</div>
```

You can also specify a language, for example:

``` html
<div
  google-add-preferred-source-btn
  data-lang="en">
</div>
```

If you do not specify a language, the default behaviour uses the
visitor's browser language. Check Google's current documentation for
supported attributes and options.

## 5. Add it to WordPress

### Option A: Use a header/footer code plugin

1.  Sign in to your WordPress dashboard.
2.  Install a reputable plugin that allows scripts to be added to the
    site header and footer.
3.  Open the plugin's code-insertion settings.
4.  Add the JavaScript library from Step 2 to the header.
5.  Save the changes.
6.  Edit the page, post template or site template where the button
    should appear.
7.  Add a **Custom HTML** block containing the button element from Step
    3.
8.  Update the page.

### Option B: Use your theme or site builder

If your theme or page builder provides a facility for adding code to the
site's `<head>`, add the JavaScript library there. Then add the button
element in a Custom HTML block or equivalent element where you want it
displayed.

Avoid editing theme files directly unless you know how to maintain the
change through theme updates. A child theme or a code-management plugin
is generally safer.

## 6. Add a direct link as an alternative

If you cannot add the JavaScript button, you can link visitors to
Google's Preferred Sources page.

Replace `example.com` with your own domain:

``` html
<a href="https://www.google.com/preferences/source?q=example.com">
  Add us as a Preferred Source on Google
</a>
```

For example, for `digitalneighbour.co.nz`:

``` html
<a href="https://www.google.com/preferences/source?q=digitalneighbour.co.nz">
  Add us as a Preferred Source on Google
</a>
```

This is a link to Google's selection experience, not an automatic
subscription. Test the link and confirm that Google resolves the
intended source before publishing it.

## 7. Test the implementation

After publishing the changes:

1.  Open the page in a fresh browser tab.
2.  Check that the button appears in the intended location.
3.  If it does not appear, check that the JavaScript library is loading
    and that the button element is present in the page HTML.
4.  Check the browser console for JavaScript errors.
5.  Test on desktop and mobile.
6.  Click the button and follow Google's on-screen instructions.
7.  Confirm that the visitor can select the correct website.

The button only provides a way for visitors to make the selection. It
does not select the site for them.

## 8. SEO best practices to support your visibility

Preferred Sources is a personalisation feature, not a guaranteed ranking
boost. Continue following sound SEO practices:

-   Publish original, helpful and accurate content.
-   Keep important pages crawlable and indexable.
-   Maintain a clear site structure and useful internal links.
-   Submit and maintain your XML sitemap in Google Search Console.
-   Monitor indexing and search performance in Search Console.
-   Keep content accurate and update it when necessary.
-   Follow Google's technical and content policies.

For AI Overviews and AI Mode, follow Google's eligibility guidance for
Search generative AI features. There is no special schema markup or
button placement that guarantees inclusion.

## 9. Official Google documentation

Always refer to Google's documentation for the latest technical
requirements and supported options:

-   [Google Search Central: Preferred
    Sources](https://developers.google.com/search/docs/appearance/preferred-sources)
-   [Google Preferred Sources selection
    page](https://www.google.com/preferences/source)

## Quick implementation checklist

-   [ ] Checked whether the website is available as a Preferred Source.
-   [ ] Added Google's JavaScript library to the page `<head>`.
-   [ ] Added the button element where visitors can find it.
-   [ ] Published the changes.
-   [ ] Tested the button on desktop and mobile.
-   [ ] Confirmed that the selection flow opens and identifies the
    correct source.
-   [ ] Added a direct link as an alternative if required.

------------------------------------------------------------------------

**Note:** Google may update the feature, its availability and its
implementation details. Check the official Google Search Central
documentation before deploying this code on a production website.
