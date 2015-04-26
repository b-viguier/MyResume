# MyResume

Simple generator for my resume, using [Sculpin](https://sculpin.io).

## How to

* `composer install`
* `vendor/bin/sculpin generate`
* Browse `output_dev/index.html`

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
