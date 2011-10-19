sailthru-python-client
====================

A simple client library to remotely access the `Sailthru REST API` as per [http://docs.sailthru.com/api](http://docs.sailthru.com/api).

By default, it will make request in `JSON` format.

Tested with `Python 2.6.x` but should work also with `>= 2.4.x`

It can make requests to following [API calls](http://docs.sailthru.com/api):

* [email](http://docs.sailthru.com/api/email)
* [send](http://docs.sailthru.com/api/send)
* [blast](http://docs.sailthru.com/api/blast)
* [template](http://docs.sailthru.com/api/template)
* [list](http://docs.sailthru.com/api/list)
* [contacts](http://docs.sailthru.com/api/contacts)
* [content](http://docs.sailthru.com/api/content)
* [alert](http://docs.sailthru.com/api/alert)
* [stats](http://docs.sailthru.com/api/stats)
* [purchase](http://docs.sailthru.com/api/purchase)
* [horizon](http://docs.sailthru.com/api/horizon)

For usage examples, you can take a look at [Ruby](https://github.com/sailthru/sailthru-ruby-client/blob/master/README.md) and [PHP](https://github.com/sailthru/sailthru-php5-client/blob/master/README.md) examples

### Installation (Tested with Python 2.7.x)
    pip install git+https://github.com/sailthru/sailthru-python-client.git#egg=sailthru-client

Examples
--------
    from sailthru import *
    
    api_key = '*******'
    api_secret = '*******'
    sailthru_client = SailthruClient(api_key, api_secret)
    response = sailthru_client.get_email('eli@sailthru.com')
    
    
