# Generating Reports

Reporting is an important part of any Gottaphish campaign. To help facilitate generating reports, there are a few options you could consider:

## Using the Web UI

The Gottaphish dashboard (Campaigns section) gives a quick overview showing the results for a particular campaign:

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

In addition to providing the results in the dashboard, you have the option to export the raw logs from Gottaphish using the "Export CSV" button at the top of the page. You could then parse these CSV files using other software such as Excel or Google Sheets.

## Using the Gottaphish reporting tool

By clicking on the Reporting section you will arrive on the Opensearch dashboard. From there you can build your own dashboard or using the default one and click on export PDF

Tips: Dont forget to click on Complete on the Web UI campaign to export the result in this Opensearch dashboard.

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

## Using GoReport

Gophish has an incredible community that has built tools around the API to help make reporting easy. A great example of this is called [GoReport](https://github.com/chrismaddalena/GoReport). Gottaphish is compatible with this product as well

[GoReport](https://github.com/chrismaddalena/GoReport), created by Github user [@chrismaddalena](https://github.com/chrismaddalena/), provides a really simple, clean way to generate reports for a given Gottaphish campaign. You can use this script to generate reports for the campaign in either CSV or DOCX format.

## Leveraging the API

If you are wanting to make custom reports, perhaps for one or more campaigns, we strongly suggest you consider leveraging the extensive [Gophish API](https://docs.getgophish.com/api-documentation/).

We have a [Python API client](https://github.com/gophish/api-client-python) that can help facilitate getting the data you need from the API. You can find the documentation for the Python API client [here](https://docs.getgophish.com/python-api-client/).
