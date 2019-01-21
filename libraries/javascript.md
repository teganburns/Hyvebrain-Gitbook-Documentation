---
description: Needs to be updated to reflect recent changes
---

# Javascript

## Include Script

!\[Needs to be updated to reflect recent changes\]\(https://img.shields.io/badge/Javascript-passing-green.svg\)

`<script src="http://cdn.hyvebrain.com/libs/js/1.0.0/hyvebrain.js"></script>`

## Minified Version 

!\[Needs to be updated to reflect recent changes\]\(https://img.shields.io/badge/Javascript-passing-green.svg\)

`<script src="http://cdn.hyvebrain.com/libs/js/1.0.0/hyvebrain.min.js"></script>`

{% code-tabs %}
{% code-tabs-item title="example.js" %}
```javascript
document.addEventListener("DOMContentLoaded", function(event) {

    // Init Hyvebrain Object
    let hb = new Hyvebrain();

    // Add XMLHttpRequest EventListeners
    hb.xml_http_request.addEventListener("load", transferComplete);
    hb.xml_http_request.addEventListener("error", transferFailed);
    hb.xml_http_request.addEventListener("abort", transferCancelled);

    // Build Request
    hb.setTextContent( 'My name is Tegan Burns. ' )
        .appendTextContent( 'I like computers.' )
        .return_natural_language_raw_data( false )
        .get_pos_tag_slave_index_list_of_token_index_list()
        .get_sentence_root_list()
        .get_text_content_token_list()
        .build()
});


// Event Listener Callbacks
function transferComplete() {
        console.log('request complete: ', JSON.parse(this.responseText) );
}

function transferFailed(evt) {
        console.log('request failed');
}

function transferCancelled(evt) {
        console.log('request cancelled');
}
```
{% endcode-tabs-item %}
{% endcode-tabs %}

