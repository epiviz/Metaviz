Metaviz
======

Metaviz is an interactive visualization tool for metagenomic data with a navigation mechanism suited for taxonomic features.

For more information, visit - http://metaviz.org

Using any PHP supported webserver
---------------------------------
Copy the Metaviz directory to the webserver configured directory. Navigate to <webserver-ip>/Metaviz/index.php on your browser.

Using PHP
---------
PHP (http://php.net/) lets your run local webservers. Navigate to localhost:8181 on your browser.
To run epiviz use:
```
php.exe -S localhost:8181 -t <location of the Metaviz directory>
```

Using Docker
-------------------

Docker-compose scripts are available for use from the following github repository URL: https://github.com/epiviz/metaviz-docker

To Compile closure
-------------------
`java -jar compiler.jar --js_output_file=metaviz-compiled-jar.js --js 'src/epiviz/**' --js '!src/epiviz/default-settings.js' --js '!src/epiviz/epivizr-settings.js' --js '!src/epiviz/standalone-settings.js' --entry_point=goog:epiviz.main`
