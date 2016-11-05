# MyResume

Simple generator for my resume, using [Sculpin](https://sculpin.io).

## How to...

### ...install

`composer install`

### ...generate HTML output

* `composer html`
* Browse `output_dev/resume.html` and/or `output_dev/motivation.html` 

### ...generate PDF output

**Require [wkhtmltopdf](http://wkhtmltopdf.org/index.html), at least version 0.12.**
On OSX, you [should use 32-bit version](https://github.com/wkhtmltopdf/wkhtmltopdf/issues/2442).

* `composer pdf`
* See `output/Viguier_CV.pdf` and/or `output/Viguier_LM.pdf` 

### ...clean generated files

`composer clean`

## Hidden data

By default, personal data are hidden.
You can add them by adding the file `app/config/sculpin_site_dev.yml` with following format

```yml
imports:
- sculpin_site.yml

hidden:
  email: email@example.com
  phone: 0123456789
  address: my address
  postal: 12345
  city: my city
  receiver:
    name: John Doe
    company: ACME
    address: USA
```
