# Landing Pages



Landing pages are the actual HTML pages that are returned to the users when they click the phishing links they receive.

Landing pages support templating, capturing credentials, and redirecting users to another website after they submit their credentials.

>

To create a landing page, click on the "Landing Pages" entry in the sidebar and click the "New Page" button.

![Landing Pages](http://imgur.com/Tg4sDId.png)

The landing page modal supports the same HTML WYSIWYG editor shown in the Templates section.

## Importing a Site From URL

A powerful feature of Gottaphish is the ability to import a site from a URL. To import a site, click the "Import Site" button.&#x20;

(beta) Instead of the open Source Gophish, Gottaphish can also use an import compatible with javascript if the content of the page only load with a JS script.&#x20;

![](http://imgur.com/uqxm6iB.png)\
After entering the URL and clicking "Import", you should see the HTML of the URL populated into the editor.

If the page imported doesn't look like the imported website, don't hesitate to copy paste the HTML code exported from the module "Save-page-we"&#x20;

{% embed url="https://addons.mozilla.org/en-US/firefox/addon/save-page-we/" %}
Extension Firefox
{% endembed %}

{% embed url="https://chrome.google.com/webstore/detail/save-page-we/dhhpefjklgkmgeafimnjhojgjamoafof" %}
Extension google chrome
{% endembed %}

## Capturing Credentials

Gottaphish makes it easy to capture credentials from the landing page. To capture credentials, simply select the checkbox that says "Capture Submitted Data".

> Note: Credentials are stored **in plaintext**. If you don't want to capture passwords, don't select the "Capture Passwords" checkbox. Gottaphish will still capture other text fields, such as usernames.

### Redirecting Users

Red team assessments are all about preventing suspicion. To prevent users from becoming suspicious after entering credentials, you may want to redirect them to the original URL.

Gottaphish makes it easy to redirect users after they submit credentials. To redirect users, enter a URL in the "Redirect To:" text field that appears after the "Capture Submitted Data" checkbox is selected.

> Note: Make sure to include the full URL (including the scheme such as http:// or https://). Otherwise, browsers may interpret the URL as being relative to the Gottaphish URL.

## Static Assets

There may be times that you want to store assets such as  CSS/JS resources. To use these in Gottaphish, just compile them and add them to the block `head.`

`You can also contact the support and we can add them for you in a static folder (like yoururl.com/static/myjsfile.js)`

The HTML `<head>` element is a container for the following elements: `<title>`, `<style>`, `<meta>`, `<link>`, `<script>`, and `<base>`.

\
&#x20;
