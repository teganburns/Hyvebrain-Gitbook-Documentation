# Python

## Installation

The easiest way to install the client library for python is with [pip](https://pypi.org/project/pip/)! The latest client library can always be found at [pypi.org/project/hyvebrain](https://pypi.org/project/hyvebrain/). More information on how to install pip can be found at [pip.pypa.io/en/stable/installing](https://pip.pypa.io/en/stable/installing/).

{% code-tabs %}
{% code-tabs-item title="user install" %}
```bash
python -m pip install --user hyvebrain # Install for user (recommended)
```
{% endcode-tabs-item %}

{% code-tabs-item title="global install" %}
```bash
python -m pip install hyvebrain # Install globally
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## Usage Example

{% code-tabs %}
{% code-tabs-item title="example.py" %}
```python
#!/usr/bin/env python

import Hyvebrain

if __name__ == '__main__':
    hb = Hyvebrain.Hyvebrain()
    hb.setTextContent( "The Turing test, developed by Alan Turing in 1950, is a test of a machine's ability to exhibit intelligent behavior equivalent to, or indistinguishable from, that of a human." )
    response = hb.get_token_index_list().get_text_content_token_list().build() 
    print( response.status_code )
    print( response.text )
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## Required Methods

### `build( )`

The `build()`method is what puts your request together in a json HTTP request for the API endpoint.

## Chaining

Due to the structure of the English Language, and how Hyvebrain is built around that, we will hardly ever call just one Hyvebrain Function. Therefore when writing the python client library it was decided that the option to chain methods should be implemented. It is recommended to only chain the Hyvebrain Function methods \(as seen on line \#8\) but all methods, except for `build()`, can be chained if desired.

{% hint style="info" %}
For more information on Chaining see: [wikipedia.org/wiki/Method\_chaining](https://en.wikipedia.org/wiki/Method_chaining)
{% endhint %}

