# Internationalization using Natural Languages (NL)

##### last update: 11:58 Saturday, May 27, 2023

## AMP instructions

- [internationalization](https://amp.dev/documentation/examples/guides/internationalization/)

## Ontomatica example using `amp-lit` and `amp-mustache`

- [RDF in 50 Words or Less](https://ontomatica.io/a/12370110501010001939/)

## AMP examples

### components --> amp-accordion

- [components](https://amp.dev/documentation/components/)
- [documentation/components/](https://github.com/ampproject/amp.dev/tree/future/pages/content/amp-dev/documentation/components/)
- [documentation/components/index.html](https://github.com/ampproject/amp.dev/blob/future/pages/content/amp-dev/documentation/components/index.html)
- [documentation/components/reference with NL pages](https://github.com/ampproject/amp.dev/tree/future/pages/content/amp-dev/documentation/components/reference)
- [extensions/amp-accordion/amp-accordion.md](https://github.com/ampproject/amphtml/blob/main/extensions/amp-accordion/amp-accordion.md)
- [amp-accordion HTML (en-US)](https://amp.dev/documentation/components/amp-accordion/)
- [Spanish; documentation/components/reference/amp-accordion-v0.1@es.md](https://github.com/ampproject/amp.dev/blob/future/pages/content/amp-dev/documentation/components/reference/amp-accordion-v0.1%40es.md)

## Our Plan

### Background

#### URN and IRI

We plan to follow URN and IRI concepts for URL labels 
  * [URN](https://en.wikipedia.org/wiki/Uniform_Resource_Name)
  * [IRI](https://en.wikipedia.org/wiki/Internationalized_Resource_Identifier)

#### IDN

We do not plan to follow internationalized domain name techniques which use language glyphs in the URL
  * [IDN](https://en.wikipedia.org/wiki/Internationalized_domain_name)

### Site partitions for mono repo

- In order to maintain a mono repo but partition site content, use a two-letter prefix
  - /aa/20-digit-identifier/
  - /ba/20-digit-identifier/
  - /ca/20-digit-identifier/
  - /da/20-digit-identifier/
  - /ea/20-digit-identifier/
  - /fa/20-digit-identifier/

- The URL will be
  - {domain}/aa/20-digit-identifier/
  - {domain}/ba/20-digit-identifier/
  - {domain}/ca/20-digit-identifier/
  - {domain}/da/20-digit-identifier/
  - {domain}/ea/20-digit-identifier/
  - {domain}/fa/20-digit-identifier/
