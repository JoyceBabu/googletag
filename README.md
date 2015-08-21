#Google Publisher Tag
---


### Introduction

In this dummy script you can find an example of googletag implementation.
I am using this approach on production, one of the advantages is that i have full control of displaying the ad.
Moreover i can easily register an event which gets triggered after my ad was rendered.

Important is that you are disabling initial loading of the ads:
```
googletag.pubads().disableInitialLoad();
```
 
If you use asynchronous execution which i highly recommend, make sure that you are pushing your code into googletag.cmd:
```
googletag.cmd.push(function() {
    // here comes your code which gets executed after googletag is ready
});
```

For more information please check out the official api:
- [Build Google Publisher Tags](https://support.google.com/dfp_sb/topic/4409240)
- [GPT API](https://developers.google.com/doubleclick-gpt/)

