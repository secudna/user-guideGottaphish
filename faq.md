# FAQ



## Events Aren't Showing Up on the Dashboard

If you are seeing emails being sent successfully, but aren't seeing events show up on the dashboard, it likely means there is a configuration error somewhere. You can follow these tips to help track it down.

**Check the Email Template**

You want to make sure you're using the `{{.URL}}` template tag when creating links in your emails. Then, when you launch a campaign, Gottaphish will fill this in with whatever you use as the "URL" field when creating the campaign.

A good way to see if this is working correctly is to send a test email to yourself when building a campaign and looking at the link. It should be the URL you used when creating the campaign with a unique `rid` parameter. So, it should look like this: `http://your_url/?rid=XXXXX`.

{% hint style="info" %}
**Tip**: Don't try to put your Gottaphish URL directly into a template. It's very important to use the `{{.URL}}` template tag, since that's how Gottaphish knows to generate the unique URL for each recipient.
{% endhint %}

****

## Submitted Form Data Isn't Being Captured

To capture data submitted through a landing page, you need to create an HTML `<form>` element on your landing page that has a few specific properties:

Here is a minimal example `<form>` element which captures data:

```markup
<form action="" method="POST">
    <input name="username" type="text" placeholder="username" />
    <input name="password" type="password" placeholder="password" />
    <input type="submit" value="Submit" />
</form>
```

There are a few things to note about this form:

* The action is `""` so that form submissions are directed to your phishing page and, therefore, to your Gottaphish server
* The form submission method is `POST`
* Each input which you expect to see in Gottaphish has a `name` attribute

Each of these should be checked when troubleshooting HTML forms that don't appear to be sending data correctly.

If you still aren't seeing your form submitted correctly, you may need to review and remove any Javascript on the page interfering with the form submission.

Finally, ensure that when saving the landing page that you have both the "Capture Submitted Data" and "Capture Passwords" (if appropriate) options checked. Otherwise, Gottaphish will remove the `name` attributes from your inputs so they aren't submitted with the form.
