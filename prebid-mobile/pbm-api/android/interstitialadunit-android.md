---
layout: page_v2
title: InterstitialAdUnit - Android
description: InterstitialAdUnit - Android
top_nav_section: prebid-mobile
nav_section: prebid-mobile
sidebarType: 2
---

# InterstitialAdUnit Object
{:.no_toc}

Use the `InterstitialAdUnit` object to create and configure an interstitial ad unit in your app.

* TOC
{:toc}

## Object

### InterstitialAdUnit

Create a new Interstitial Ad Unit associated with a Prebid Server configuration ID.

**Parameters**

`configId`: Prebid Server configuration ID.

## Methods

`InterstitialAdUnit` inherits all methods from the [AdUnit]({{site.baseurl}}/prebid-mobile/api/adunit-android.html) object.

## Example

```
InterstitialAdUnit interstitialAdUnit = new InterstitialAdUnit("PREBID_SERVER_CONFIGURATION_ID");
interstitialAdUnit.setUserKeyword("my_key", "my_value");
interstitialAdUnit.fetchDemand(publisherAdRequest, new onCompleteListener() {
    @Override
    public void onComplete(ResultCode resultCode) {
        dfpInterstitial.loadAd(publisherAdRequest);
    }
});
```

## Related Topics

- [Prebid Mobile API - Android]({{site.baseurl}}/prebid-mobile/api/pbm-api-android.html)
- [Banner Ad Unit]({{site.baseurl}}/prebid-mobile/api/banneradunit-android.html)
- [Ad Unit]({{site.baseurl}}/prebid-mobile/api/adunit-android.html)
- [Result Codes]({{site.baseurl}}/prebid-mobile/api/pbm-api-result-codes-android.html)
- [Targeting Parameters]({{site.baseurl}}/prebid-mobile/api/pbm-targeting-params-android.html)
- [Prebid Mobile Object]({{site.baseurl}}/prebid-mobile/api/prebidmobile-object-android.html)
- [Prebid Mobile API - iOS]({{site.baseurl}}/prebid-mobile/api/pbm-api-ios.html)