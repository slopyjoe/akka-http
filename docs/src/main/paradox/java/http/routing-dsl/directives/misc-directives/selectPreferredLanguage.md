<a id="selectpreferredlanguage-java"></a>
# selectPreferredLanguage

## Description

Inspects the request's `Accept-Language` header and determines,
which of a given set of language alternatives is preferred by the client according to content negotiation rules
defined by [http://tools.ietf.org/html/rfc7231#section-5.3.5](http://tools.ietf.org/html/rfc7231#section-5.3.5).

If there are several best language alternatives that the client has equal preference for
(even if this preference is zero!) the order of the arguments is used as a tie breaker (first one wins).

## Example

@@snip [MiscDirectivesExamplesTest.java](../../../../../../../test/java/docs/http/javadsl/server/directives/MiscDirectivesExamplesTest.java) { #selectPreferredLanguage }