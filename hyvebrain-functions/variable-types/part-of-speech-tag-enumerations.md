# Part Of Speech Tag Enumerations

## Synopsis

There are currently 13 Part Of Speech Tag Enumerations. Each enumeration links a [Parts Of Speech Tag Type ](../../definitions/parts-of-speech/)to an integer.

{% code-tabs %}
{% code-tabs-item title="Part Of Speech Tag Enumerations" %}
```cpp
enum PartOfSpeech_Tag {
  PartOfSpeech_Tag_UNKNOWN = 0,
  PartOfSpeech_Tag_ADJ = 1,
  PartOfSpeech_Tag_ADP = 2,
  PartOfSpeech_Tag_ADV = 3,
  PartOfSpeech_Tag_CONJ = 4,
  PartOfSpeech_Tag_DET = 5,
  PartOfSpeech_Tag_NOUN = 6,
  PartOfSpeech_Tag_NUM = 7,
  PartOfSpeech_Tag_PRON = 8,
  PartOfSpeech_Tag_PRT = 9,
  PartOfSpeech_Tag_PUNCT = 10,
  PartOfSpeech_Tag_VERB = 11,
  PartOfSpeech_Tag_X = 12,
  PartOfSpeech_Tag_AFFIX = 13,
};
```
{% endcode-tabs-item %}
{% endcode-tabs %}

{% hint style="info" %}
When specifying a Part Of Speech Tag Type in a POST request, as function argument, you can use the capital type name or the integer. \( "NOUN" or "6" \)
{% endhint %}

