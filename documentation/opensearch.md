# OpenSearch

OpenSearch is a family of software consisting of a search engine, and OpenSearch Dashboards, a data visualization dashboard for that search engine.

## View your campaign dashboard

To view your campaign dashboard, you must go to the “Reporting” tab.

<figure><img src="../.gitbook/assets/image.png" alt="" width="473"><figcaption></figcaption></figure>

Then you need to click on “Log in with single sign-on”.

<figure><img src="../.gitbook/assets/image (1).png" alt="" width="437"><figcaption></figcaption></figure>

Then you will arrive on the Keycloack connection page, you will need to log in with your connection details.

<figure><img src="../.gitbook/assets/image (2).png" alt="" width="563"><figcaption></figcaption></figure>

Then you have to go to Gottaphish reporting.

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Then on "discover".&#x20;

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

Then on "Campagne all".&#x20;

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

You will arrive on a dashboard like this below. You can view the different OS, the percentage of emails opened, the percentage of data transmitted and the percentage of clicks.

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

At the top left in filtered then in "edit as Query DSL" you can filter for example all campaigns using "Campaign".

<figure><img src="../.gitbook/assets/image (9).png" alt="" width="563"><figcaption></figcaption></figure>

```
{
  "query": {
    "wildcard": {
      "campaign_name.keyword": {
        "value": "Campagne*"
      }
    }
  }
}
```
