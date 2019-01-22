# Poltio Embed Widgets 

## Dynamic Resizing via Poltio Resizer SDK 

If you want to use Poltio Widgets in your page multiple times and don't want to give height information for all the widgets, you can use resizer sdk implementation. 

Add the following line to somewhere in your HTML once and it will dedect Poltio Widgets and change their height attributes to fit the page. It will do all the calculations inside of the widget so it will not impact your page performance. 

```html
<script type="text/javascript" src="//sdk.poltio.com/prod/resizer.js" defer></script>
```


## Tracking Votes With Your Own IDs

By default all votes will have a Poltio User ID assigned to them. If you also want to track and match your own user ids with poltio user ids, you add a unique id to poltio widget source as a query string parameter (*uuid*)

```html
<figure class="op-interactive">
    <iframe 
        id="poltio-embed-poll-148692" 
        class="poltio-embed" 
        src="https://www.poltio.com/e/poll/148692?uuid=XX" 
        width="100%" 
        height="500" 
        frameBorder="0" 
        allowFullScreen="allowfullscreen" 
        scrolling="yes" 
        title="Embed">
    </iframe>
</figure>
```

Here in this example, you need to update the XX with a unique id to identify that user. You can use your own user ids or create unique ids just to use in poltio widgets. 
This uuid information will be only available in your Poltio Pro dashboards as **Publisher ID**
