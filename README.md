[![Build status](https://travis-ci.org/AqoviaElements/epi-cms-property.svg?branch=master)](https://travis-ci.org/AqoviaElements/epi-cms-property)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/AqoviaElements/epi-cms-property)

## &lt;epi-cms-property&gt;

`<epi-cms-property>` is a web component used to retrieve a page property from a page within an Episerver CMS website.

### Usage:

An ancestor element with "cms-page-id" attribute should be set on each page on which the web component is used, containing the page's Page ID.
Then, simply provide the component with the name of the page property as an attribute, and the content will be rendered:

```html
<body cms-page-id="pageId">
    <epi-cms-property property-name="nameOfProperty"></epi-cms-property>
</body>
```

Note. The endpoint at which the component will attempt to retrieve the Episerver content from, is:
`/api/episerver/page/[pageId]/property/[propertyName]`

