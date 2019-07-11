---
title: "Feed Reader"
date: 2019-07-04T05:53:08-04:00
draft: false
weight: 65
---

<img class="screenshot" src="/imgs/modules/feedreader.png" width="320" height="94" alt="feedreader screenshot" />

A rudimentary RSS & Atom feed reader.

## Configuration

```yaml
feedreader:
  enabled: true
  feeds:
  - https://news.ycombinator.com/rss
  - http://feeds.reuters.com/Reuters/worldNews
  feedLimit: 10
  position:
    top: 4
    left: 1
    height: 1
    width: 2
  refreshInterval: 14400
```

{{% attributes %}}
  {{< attributes/border >}}
  {{< attributes/enabled >}}
  {{< attributes/custom name="feedLimit" description="The number of stories from each feed to be displayed. Default is `-1`, which will display all available stories." value="Any integer greater than zero. Values zero or less will display all." >}}
  {{< attributes/custom name="feeds" description="List of RSS or Atom feed URLs." value="" >}}
  {{< attributes/focusChar >}}
  {{< attributes/position >}}
  {{< attributes/refreshInterval >}}
{{% /attributes %}}

## Keyboard Commands

<span class="caption">Key:</span> `[return]` <br />
<span class="caption">Action:</span> Open the selected story in the browser.

<span class="caption">Key:</span> `j` <br />
<span class="caption">Action:</span> Select the next story in the list.

<span class="caption">Key:</span> `k` <br />
<span class="caption">Action:</span> Select the previous story in the list.

<span class="caption">Key:</span> `o` <br />
<span class="caption">Action:</span> Open the selected story in the browser.

<span class="caption">Key:</span> `r` <br />
<span class="caption">Action:</span> Refresh the data.

<span class="caption">Key:</span> `↓` <br />
<span class="caption">Action:</span> Select the next story in the list.

<span class="caption">Key:</span> `↑` <br />
<span class="caption">Action:</span> Select the previous story in the list.

{{% sourcePath module="feedreader" %}}