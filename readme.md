# PHP XML Sitemap

*Version 1.0*

## In short

- Really small
- Really simple to use
- No dependencies

## Usage

```php
include __DIR__ . '/php-xml-sitemap.php';

$sitemap = new PHPXMLSitemap('https://example.com');
$sitemap->add('/', '1.0', 'daily', '2019-03-20');
$sitemap->add('about');
$sitemap->render();
```

It will generate something like below:

```text
<?xml version="1.0" encoding="utf-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <priority>1.0</priority>
    <changefreq>daily</changefreq>
    <lastmod>2019-03-20</lastmod>
    <loc>https://example.com</loc>
  </url>
  <url>
    <priority>0.5</priority>
    <changefreq>daily</changefreq>
    <lastmod>2019-04-22</lastmod>
    <loc>https://example.com/about</loc>
  </url>
</urlset>
```

## Donate

Donate to [DevoneraAB](https://www.paypal.me/DevoneraAB) if you want.

## License

MIT