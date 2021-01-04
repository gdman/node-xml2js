node-xml2js-stringify
===========

This is a fork of the excellent [node-xml2js](https://github.com/Leonidas-from-XIV/node-xml2js) module by [Leonidas-from-XIV](https://github.com/Leonidas-from-XIV).

The only difference in this fork is the `stringify` builder option that is now passed through [node-xml2js](https://github.com/Leonidas-from-XIV/node-xml2js) to [xmlbuilder-js](https://github.com/oozcitak/xmlbuilder-js).

Forked from version 0.4.23.


Background
---
The following issues are tracked against node-xml2js:

 * [Unicode character inside attributes - #165](https://github.com/Leonidas-from-XIV/node-xml2js/issues/165)
 * [Handling HTML Entities - #450](https://github.com/Leonidas-from-XIV/node-xml2js/issues/450)

A [PR](https://github.com/Leonidas-from-XIV/node-xml2js/pull/451) has been raised by [boxfoot](https://github.com/boxfoot) to pass this option through the `stringify` option to `xmlbuilder-js` but this has been declined for the reasons outlined in [#450](https://github.com/Leonidas-from-XIV/node-xml2js/issues/450).

Like [boxfoot](https://github.com/boxfoot), I need to be able to be explicit in the format of XML output so have created this forked repository.


Extra option for the `Builder` class
---
  * `stringify` (default: `null`): provides a set of functions which tell XMLBuilder how to convert values into strings.

  See [docs](https://github.com/oozcitak/xmlbuilder-js/wiki) and [XMLStringifier](https://github.com/oozcitak/xmlbuilder-js/blob/master/src/XMLStringifier.coffee)