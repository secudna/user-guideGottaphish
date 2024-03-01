# Landing Pages



Landing pages are the actual HTML pages that are returned to the users when they click the phishing links they receive.

Landing pages support templating, capturing credentials, and redirecting users to another website after they submit their credentials.



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

Gottaphish makes it easy to capture credentials from the landing page. To capture credentials, simply check the “Capture submitted data” box but you will capture all except the password. Whereas if you want to capture passwords by checking the “Capture passwords” box.

> Note: Credentials are stored **in plaintext**. If you don't want to capture passwords, don't select the "Capture Passwords" checkbox. Gottaphish will still capture other text fields, such as usernames.

It is possible to check the “capture password strength” box which allows you to evaluate the strength of the password on a score of 1 to 100.

### Redirecting Users

Red team assessments are primarily intended to prevent suspicion. To prevent users from becoming suspicious after entering their credentials, you may want to redirect them to the original URL. Gottaphish makes it easy to redirect users after submitting their credentials. This is why we have set up a redirection page which is the following "https://speed-training.gottaphish.com/fr/trap?rid=\{{.RId\}}" which warns the user it's being trapped.

<figure><img src="../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

## Static Assets

There may be times that you want to store assets such as  CSS/JS resources. To use these in Gottaphish, just compile them and add them to the block `head.`

`You can also contact the support and we can add them for you in a static folder (like yoururl.com/static/myjsfile.js)`

The HTML `<head>` element is a container for the following elements: `<title>`, `<style>`, `<meta>`, `<link>`, `<script>`, and `<base>`.



## Example Landing page&#x20;

This dynamic landing page will adapt depending on the company or tools the person is using. The page will adapt to resemble the desired service. It will consist of a connection space, the name and logo of the company or tool

\
&#x20;
