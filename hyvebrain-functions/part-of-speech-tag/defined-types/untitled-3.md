---
description: Alias for functions that retrieve a defined part of speech tag type
---

# get\_pos\_tag\_-\_str\(\)

## Parameters

{% tabs %}
{% tab title="Argument" %}
\*\*\*\*[**`val_vec_int_si`**](../../variable-types/val_vec_int_si.md)

If no **`val_vec_int_si`** is supplied the argument will default to **`get_current_sentence_index()`**
{% endtab %}

{% tab title="Returns" %}
\*\*\*\*[**`val_vec_int_ti`**](../../variable-types/val_vec_int_ti.md)
{% endtab %}

{% tab title="Notes" %}
The content of the return value varies based on the function being called. For example if you were to use the **`get_pos_tag_NOUN()`** function it would return a vector of token indexes where the [**`val_pos_tag`**](../../variable-types/val_pos_tag.md) is a [**NOUN**](../../../definitions/parts-of-speech/noun.md).
{% endtab %}
{% endtabs %}

## Operation

Iterates through each token index \([**`val_int_ti`**](../../variable-types/val_int_ti.md)\) in the provided sentence index \([**`val_int_si`**](../../variable-types/val_int_si.md)\). For each token index it will check the part of speech tag \([**`val_pos_tag`**](../../variable-types/val_pos_tag.md)\) type. If the part of speech tag type matches the defined type.

The content of the return value varies based on the function being called. For example if you were to use the **`get_pos_tag_NOUN()`** function it would return a vector of token indexes where the [**`val_pos_tag`**](../../variable-types/val_pos_tag.md) is a [NOUN](../../../definitions/parts-of-speech/noun.md).

## Defined Functions

| Function Name | Defined Type |
| :--- | :--- |
| get\_pos\_tag\_UNKNOWN\(\) | [UNKNOWN](../../../definitions/parts-of-speech/unknown.md) |
| get\_pos\_tag\_ADJ\(\) | [ADJ](../../../definitions/parts-of-speech/adj.md) |
| get\_pos\_tag\_ADP\(\) | [ADP](../../../definitions/parts-of-speech/adp.md) |
| get\_pos\_tag\_ADV\(\) | [ADV](../../../definitions/parts-of-speech/adv.md) |
| get\_pos\_tag\_CONJ\(\) | [CONJ](../../../definitions/parts-of-speech/conj.md) |
| get\_pos\_tag\_DET\(\) | [DET](../../../definitions/parts-of-speech/det.md) |
| get\_pos\_tag\_NOUN\(\) | [NOUN](../../../definitions/parts-of-speech/noun.md) |
| get\_pos\_tag\_NUM\(\) | [NUM](../../../definitions/parts-of-speech/num.md) |
| get\_pos\_tag\_PRON\(\) | [PRON](../../../definitions/parts-of-speech/pron.md) |
| get\_pos\_tag\_PRT\(\) | [PRT](../../../definitions/parts-of-speech/prt.md) |
| get\_pos\_tag\_PUNCT\(\) | [PUNCT](../../../definitions/parts-of-speech/punct.md) |
| get\_pos\_tag\_VERB\(\) | [VERB](../../../definitions/parts-of-speech/verb.md) |
| get\_pos\_tag\_X\(\) | [X](../../../definitions/parts-of-speech/x.md) |
| get\_pos\_tag\_AFFIX\(\) | [AFFIX](../../../definitions/parts-of-speech/affix.md) |

