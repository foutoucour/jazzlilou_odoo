# jazzlilou_odoo

## Production

``` shell 
setenv COMPOSE_FILE=docker-compose.prod.yml
docker-compose down
docker-compose up -d
```
That puts two services up, an odoo stack, and a wordpress stack.

### urls
* odoo: https://edithcourtial.com
* wordpress: http://edithcourtial.com:9000

## Odoo

### Wkhtmltopdf setup

I needed to setup the web.base.url to https://edithcourtial.com:8069
so wkhtmltopdf is not lost in the urls.
in settings:system parameters
see https://www.odoo.com/fr_FR/forum/aide-1/question/where-to-specify-the-parameter-of-wkhtmltopdf-in-odoo-94706