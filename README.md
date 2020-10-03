# AJAX proxy for stolperstein-bonn

**Obsolete now**

OpenStreetMap supports different kinds of specification for the **image**
attribute. It can be the URL of an image, the URL of a page of an image or
**File:**, the latter referring to an image on WikiMedia Commons.

For finding image URLs for the latter, the WikiMedia API can be used. However,
there is one issue: The same-origin security policy imposed by browsers. You
cannot directly use the API from another domain. You however can use a proxy
located on the same machine that forwards your requests to a MediaWiki and the
answers sent by it to your machine.

This is what this program is all about. It essentially is the [Guide4You AJAX
proxy](https://github.com/KlausBenndorf/guide4you-proxy) I wrote for the
company I work at, customized to access precisely one particular URL.

Note that the Guide4You AJAX proxy in turn is based on [AJAX Cross Domain
(PHP) Proxy](https://github.com/softius/php-cross-domain-proxy) by Iacovos
Constantinou.
