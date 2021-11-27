# php56_chinese_converter
php56中文簡繁轉換

# 安裝教程

將mediawiki.rar下載到本地解壓,將壓縮包根目錄下的mediawiki-zhconverter.inc.php複製到php程序中,然後在程序中设置MediaWiki路径,及引用mediawiki-zhconverter,
```php
define("MEDIAWIKI_PATH", "/var/lib/mediawiki-1.14.0/");
require_once "mediawiki-zhconverter.inc.php";
```

# 轉換示例
```php
$converter = new MediaWikiZhConverter();
$converter->convert($k, "zh-tw")  //轉換成繁體
$converter->convert($k, "zh-cn")  //轉換成簡體
```
