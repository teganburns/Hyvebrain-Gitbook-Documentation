---
description: Alias for functions that retrieve a defined part of speech tag type
---

# get\_pos\_tag\_-\_str\_list\(\)

## Parameters

{% tabs %}
{% tab title="Argument" %}
[`val_vec_int_si`](../../variable-types/val_vec_int_si.md)

If no `val_vec_int_si` is supplied the argument will default to `get_sentence_index_list()`
{% endtab %}

{% tab title="Returns" %}
[`val_vec_str`](../../variable-types/val_vec_str.md)
{% endtab %}

{% tab title="Notes" %}
The content of the return value varies based on the function being called. For example if you were to use the `get_pos_tag_NOUN_list()` function it would return a vector of strings where the [`val_pos_tag`](../../variable-types/val_pos_tag.md) is a [**NOUN**](../../../definitions/parts-of-speech/noun.md).
{% endtab %}
{% endtabs %}

## Operation

Iterates through each sentence \([`val_int_si`](../../variable-types/val_int_si.md)\) in the provided vector of sentences \([`val_vec_int_si`](../../variable-types/val_vec_int_si.md)\). Then iterates through each token \([`val_int_ti`](../../variable-types/val_int_ti.md)\) in the aforementioned sentence \([`val_int_si`](../../variable-types/val_int_si.md)\). For each token it will check the part of speech tag \([`val_pos_tag`](../../variable-types/val_pos_tag.md)\) type. If the part of speech tag type matches the defined type, then the token's string value will be appended to a vector. When there are no more tokens in the sentence and no more sentences in the vector of sentences to iterate though the vector is returned.

{% hint style="success" %}
**Pro-tip**: These functions are almost the same as [`get_pos_tag_-_list()`](get_pos_tag_-_list.md)

Instead of returning a vector of token indexes \([`val_vec_int_ti`](../../variable-types/val_vec_int_ti.md)\) the tokens are represented as a vector of strings \([`val_vec_str`](../../variable-types/val_vec_str.md)\)
{% endhint %}

## Defined Functions

| Function Name | Defined Type |
| :--- | :--- |
| get\_pos\_tag\_UNKNOWN\_str\_list\(\) | [UNKNOWN](../../../definitions/parts-of-speech/unknown.md) |
| get\_pos\_tag\_ADJ\_str\_list\(\) | [ADJ](../../../definitions/parts-of-speech/adj.md) |
| get\_pos\_tag\_ADP\_str\_list\(\) | [ADP](../../../definitions/parts-of-speech/adp.md) |
| get\_pos\_tag\_ADV\_str\_list\(\) | [ADV](../../../definitions/parts-of-speech/adv.md) |
| get\_pos\_tag\_CONJ\_str\_list\(\) | [CONJ](../../../definitions/parts-of-speech/conj.md) |
| get\_pos\_tag\_DET\_str\_list\(\) | [DET](../../../definitions/parts-of-speech/det.md) |
| get\_pos\_tag\_NOUN\_str\_list\(\) | [NOUN](../../../definitions/parts-of-speech/noun.md) |
| get\_pos\_tag\_NUM\_str\_list\(\) | [NUM](../../../definitions/parts-of-speech/num.md) |
| get\_pos\_tag\_PRON\_str\_list\(\) | [PRON](../../../definitions/parts-of-speech/pron.md) |
| get\_pos\_tag\_PRT\_str\_list\(\) | [PRT](../../../definitions/parts-of-speech/prt.md) |
| get\_pos\_tag\_PUNCT\_str\_list\(\) | [PUNCT](../../../definitions/parts-of-speech/punct.md) |
| get\_pos\_tag\_VERB\_str\_list\(\) | [VERB](../../../definitions/parts-of-speech/verb.md) |
| get\_pos\_tag\_X\_str\_list\(\) | [X](../../../definitions/parts-of-speech/x.md) |
| get\_pos\_tag\_AFFIX\_str\_list\(\) | [AFFIX](../../../definitions/parts-of-speech/affix.md) |

