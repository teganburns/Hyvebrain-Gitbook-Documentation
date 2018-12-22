# Example

## Hello World

For this example we will breakdown the "[Hello\_World.sh](example.md#hello-world)" script below. The script will make a cURL request to **api.hyvebrain.com/v/testing/.** The **text\_content** in the request is the first sentence on the Wikipedia page for [Turing Test](https://en.wikipedia.org/wiki/Turing_test). The script also requests that the **get\_pos\_tag\_NOUN\_list** function is called. Copy and paste the code into a bash terminal to see the API  in action.

{% code-tabs %}
{% code-tabs-item title="Hello\_World.sh" %}
```bash
#! /bin/bash
curl -s --header "Content-Type: application/json" \
--request POST "https://api.hyvebrain.com/v/testing/" \
--data '{"text_content":"The Turing test, developed by Alan Turing in 1950, is a test of a machine'\''s ability to exhibit intelligent behavior equivalent to, or indistinguishable from, that of a human.","functions": [ "get_pos_tag_NOUN_list" ] }'

```
{% endcode-tabs-item %}
{% endcode-tabs %}

{% hint style="warning" %}
Notice the use of escape charters in the code above \(machine's\). This is necessary for bash to execute the request correctly.
{% endhint %}

## Request

Now let's breakdown the request into different parts to better understand each section!

### URL Endpoint

The url endpoint is the address that the request will be sent to. On line number two of the ["Hello\_World.sh"](example.md#hello-world) example \(above\) we see the url endpoint : `https://api.hyvebrain.com/v/testing/`There is currently only one endpoint for this API but that may change in the future. 

{% hint style="warning" %}
All requests made must be a HTTP POST request. All other HTTP request types will result in an error.
{% endhint %}

### **Content Body**

The content body is where you will specify the parameters of the request. For this part we will look at the four different parameters can used. 

The first two of these are the content to be analyzed. This can either be **text\_content** or **natural\_language\_raw\_data.** 

### text\_content

**text\_content** is a string. This string can be words or sentences that you want to perform functions on. 

In the "[Hello\_World.sh](example.md#hello-world)" example you can see on line four the **text\_content** is: _`"The Turing test, developed by Alan Turing in 1950, is a test of a machine's ability to exhibit intelligent behavior equivalent to, or indistinguishable from, that of a human."`_

### natural\_language\_raw\_data

**natural\_language\_raw\_data** is a json object. This json object is returned when requested via the [**return\_natural\_language\_raw\_data**](example.md#return_natural_language_raw_data). 

If you have received this json object via [**return\_natural\_language\_raw\_data**](example.md#return_natural_language_raw_data) from a previous request and would like to execute functions on the same [**text\_content**](example.md#text_content) use the key **natural\_language\_raw\_data** with the json object as the value.

### functions

**functions** is an array. This array contains function names to be executed in series of back to front. On line four of the "[Hello\_World.sh](example.md#hello-world)" example we only executed one function. `"functions": [ "get_pos_tag_NOUN_list" ]`

There are a lot of different functions available. These functions are what make Hyvebrain unique. To read more check out the section on **Hyvebrain Functions**.

### return\_natural\_language\_raw\_data

**return\_natural\_language\_raw\_data** is an integer. If this integer is greater than zero the response will contain the **natural\_language\_raw\_data** json object.

If you are making requests on the same [**text\_content**](example.md#text_content) more then once this will decrease the API response time. In addition, these requests are free and have no limitations.

## **Response**

Your response to the "Hello\_World.sh" example should look similar to the example below.

{% code-tabs %}
{% code-tabs-item title="Response.json" %}
```javascript
{
  "retval": 0,
  "result": {
    "val_int_ti": null,
    "val_int_si": null,
    "val_pos_tag": null,
    "val_depe_label": null,
    "val_str": null,
    "val_vec_int_ti": [
      1,
      2,
      6,
      7,
      13,
      16,
      18,
      22,
      33
    ],
    "val_vec_int_si": [
      0
    ],
    "val_vec_pos_tag": [
      null
    ],
    "val_vec_depe_label": [
      null
    ],
    "val_vec_str": [
      null
    ],
    "natural_language_raw_data": null
  }
}

```
{% endcode-tabs-item %}
{% endcode-tabs %}

### Checking for Errors

When making a request you need to check three things before working with the data.

1. **Check the HTTP response code is "**[**200 OK**](https://en.wikipedia.org/wiki/List_of_HTTP_status_codes#2xx_Success)**".** 
2. **Check the "retval".** Line two in the "[Response.json](example.md#response)" shows the **retval** \(return value\) is zero. If the **retval** is anything other than zero then there is an error.
3. **Check the "errmsg".** The **errmsg** key is only present if an error occurs.

### Result Object

From line three to thirty three in the "[Response.json](example.md#response)" you can see the **result object**. The **result object** contains one of each [**Variable Type**](hyvebrain-functions/variable-types/)**.** 

{% hint style="info" %}
Be sure to read more on [**Hyvebrain Variable Types**](hyvebrain-functions/variable-types/) to better understand the response data.
{% endhint %}



