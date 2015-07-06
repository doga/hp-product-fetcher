# hp-product-fetcher

## Description
`hp-product-fetcher` is a standalone script that fetches product pages from the HP website 
and writes them into a directory.
As argument, this script takes one or more HP webpage URLs and a directory path.

### Usage
    `hp-product-fetcher [options] hp_webpage_url... directory`

### Options
    -d, --delay D                    Set the delay between requests, in seconds.
                                     The default value is 2.
    -r, --requests R                 Set the maximum number of web requests that can be issued
                                     during the session.
    -p, --products P                 Set the maximum number of product pages that can be downloaded
                                     during the session.
    -v, --[no-]verbose               Run verbosely.
    -V, --version                    Display the current version number and exit.
    -h, --help                       Display this help message and exit.

### Usage example
    ```hp-product-fetcher --products 100 --verbose \
      'http://www.hp.com/country/us/en/hho/welcome.html' \
      ~/HP_data_audit/Available_HP_products```

## Installation

1. Install [ruby](https://www.ruby-lang.org/en/) on your machine.
2. Put the `hp-product-fetcher` script in a directory on your machine. That's it!

## System requirements
`hp-product-fetcher` only depends on ruby 2.1 or later. It has been tested on Linux,
and it will also run on Windows, Apple's OS X, and many UNIX-like operating systems.

## Support
You can visit [the GitHub repository](https://github.com/doga/hp-product-fetcher)
to file a bug report and, even better, send me a pull request if you would like
to contribute.
