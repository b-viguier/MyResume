# MyResume

Simple generator for my resume, using [Sculpin](https://sculpin.io).

## How to...

### ...install

`composer install`

### ...generate HTML output

* `composer html`
* Browse `output_dev/index.html`

### ...generate PDF output

**Require [wkhtmltopdf](http://wkhtmltopdf.org/index.html), at least version 0.12**

* `composer pdf`
* See `output/CV_Viguier.pdf`

## Hidden data

By default, personal data are hidden.
You can add them by adding the file `app/config/sculpin_site_dev.yml` with following format

```yml
imports:
- sculpin_site.yml

hidden:
  email: email@example.com
  phone: 0123456789
  address: France
```
