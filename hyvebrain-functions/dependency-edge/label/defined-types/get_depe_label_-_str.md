---
description: Alias for functions that retrieve a defined dependency edge label type
---

# get\_depe\_label\_-\_str\(\)

## Parameters

{% tabs %}
{% tab title="Argument" %}
[`val_int_si`](../../../variable-types/val_int_si.md)

If no `val_int_si` is supplied the argument will default to `get_current_sentence_index()`
{% endtab %}

{% tab title="Returns" %}
[`val_vec_str`](../../../variable-types/val_vec_str.md)
{% endtab %}

{% tab title="Notes" %}
The content of the return value varies based on the function being called. For example if you were to use the `get_depe_label_POBJ_str()` function it would return a vector of strings where the [`val_depe_label`](../../../variable-types/val_depe_label.md) is a [**POBJ**](../../../../definitions/dependency-labels/pobj.md).
{% endtab %}
{% endtabs %}

## Operation

Iterates through each token \([`val_int_ti`](https://docs.hyvebrain.com/~/drafts/-LUwZHJukv0KMhgvdvUK/primary/hyvebrain-functions/variable-types/val_int_ti)\) in the provided sentence \([`val_int_si`](https://docs.hyvebrain.com/~/drafts/-LUwZHJukv0KMhgvdvUK/primary/hyvebrain-functions/variable-types/val_int_si)\). For each token it will check the dependency edge label \([`val_depe_label`](../../../variable-types/val_depe_label.md)\) type. If the dependency edge label type matches the defined type the token's string value will be appended to a vector. When there are no more tokens in the sentence to iterate though the vector is returned.

{% hint style="success" %}
🥇 **Pro-tip**: These functions are almost the same as [`get_depe_label_-()`](get_depe_label_.md)

Instead of returning a vector of token indexes \([`val_vec_int_ti`](../../../variable-types/val_vec_int_ti.md)\) the tokens are represented as a vector of strings \([`val_vec_str`](../../../variable-types/val_vec_str.md)\)
{% endhint %}

## Defined Functions

| Function Name | Defined Type |
| :--- | :--- |
| get\_depe\_label\_UNKNOWN\_str\(\) | [UNKNOWN](../../../../definitions/dependency-labels/unknown.md) |
| get\_depe\_label\_ABBREV\_str\(\) | [ABBREV](../../../../definitions/dependency-labels/abbrev.md) |
| get\_depe\_label\_ACOMP\_str\(\) | [ACOMP](../../../../definitions/dependency-labels/acomp.md) |
| get\_depe\_label\_ADVCL\_str\(\) | [ADVCL](../../../../definitions/dependency-labels/advcl.md) |
| get\_depe\_label\_ADVMOD\_str\(\) | [ADVMOD](../../../../definitions/dependency-labels/advmod.md) |
| get\_depe\_label\_AMOD\_str\(\) | [AMOD](../../../../definitions/dependency-labels/amod.md) |
| get\_depe\_label\_APPOS\_str\(\) | [APPOS](../../../../definitions/dependency-labels/appos.md) |
| get\_depe\_label\_ATTR\_str\(\) | [ATTR](../../../../definitions/dependency-labels/attr.md) |
| get\_depe\_label\_AUX\_str\(\) | [AUX](../../../../definitions/dependency-labels/aux.md) |
| get\_depe\_label\_AUXPASS\_str\(\) | [AUXPASS](../../../../definitions/dependency-labels/auxpass.md) |
| get\_depe\_label\_CC\_str\(\) | [CC](../../../../definitions/dependency-labels/cc.md) |
| get\_depe\_label\_CCOMP\_str\(\) | [CCOMP](../../../../definitions/dependency-labels/ccomp.md) |
| get\_depe\_label\_CONJ\_str\(\) | [CONJ](../../../../definitions/dependency-labels/conj.md) |
| get\_depe\_label\_CSUBJ\_str\(\) | [CSUBJ](../../../../definitions/dependency-labels/csubj.md) |
| get\_depe\_label\_CSUBJPASS\_str\(\) | [CSUBJPASS](../../../../definitions/dependency-labels/csubjpass.md) |
| get\_depe\_label\_DEP\_str\(\) | [DEP](../../../../definitions/dependency-labels/dep.md) |
| get\_depe\_label\_DET\_str\(\) | [DET](../../../../definitions/dependency-labels/det.md) |
| get\_depe\_label\_DISCOURSE\_str\(\) | [DISCOURSE](../../../../definitions/dependency-labels/discourse.md) |
| get\_depe\_label\_DOBJ\_str\(\) | [DOBJ](../../../../definitions/dependency-labels/dobj.md) |
| get\_depe\_label\_EXPL\_str\(\) | [EXPL](../../../../definitions/dependency-labels/expl.md) |
| get\_depe\_label\_GOESWITH\_str\(\) | [GOESWITH](../../../../definitions/dependency-labels/goeswith.md) |
| get\_depe\_label\_IOBJ\_str\(\) | [IOBJ](../../../../definitions/dependency-labels/iobj.md) |
| get\_depe\_label\_MARK\_str\(\) | [MARK](../../../../definitions/dependency-labels/mark.md) |
| get\_depe\_label\_MWE\_str\(\) | [MWE](../../../../definitions/dependency-labels/mwe.md) |
| get\_depe\_label\_MWV\_str\(\) | [MWV](../../../../definitions/dependency-labels/mwv.md) |
| get\_depe\_label\_NEG\_str\(\) | [NEG](../../../../definitions/dependency-labels/neg.md) |
| get\_depe\_label\_NN\_str\(\) | [NN](../../../../definitions/dependency-labels/nn.md) |
| get\_depe\_label\_NPADVMOD\_str\(\) | [NPADVMOD](../../../../definitions/dependency-labels/npadvmod.md) |
| get\_depe\_label\_NSUBJ\_str\(\) | [NSUBJ](../../../../definitions/dependency-labels/nsubj.md) |
| get\_depe\_label\_NSUBJPASS\_str\(\) | [NSUBJPASS](../../../../definitions/dependency-labels/nsubjpass.md) |
| get\_depe\_label\_NUM\_str\(\) | [NUM](../../../../definitions/dependency-labels/num.md) |
| get\_depe\_label\_NUMBER\_str\(\) | [NUMBER](../../../../definitions/dependency-labels/number.md) |
| get\_depe\_label\_P\_str\(\) | [P](../../../../definitions/dependency-labels/p.md) |
| get\_depe\_label\_PARATAXIS\_str\(\) | [PARATAXIS](../../../../definitions/dependency-labels/parataxis.md) |
| get\_depe\_label\_PARTMOD\_str\(\) | [PARTMOD](../../../../definitions/dependency-labels/partmod.md) |
| get\_depe\_label\_PCOMP\_str\(\) | [PCOMP](../../../../definitions/dependency-labels/pcomp.md) |
| get\_depe\_label\_POBJ\_str\(\) | [POBJ](../../../../definitions/dependency-labels/pobj.md) |
| get\_depe\_label\_POSS\_str\(\) | [POSS](../../../../definitions/dependency-labels/poss.md) |
| get\_depe\_label\_POSTNEG\_str\(\) | [POSTNEG](../../../../definitions/dependency-labels/postneg.md) |
| get\_depe\_label\_PRECOMP\_str\(\) | [PRECOMP](../../../../definitions/dependency-labels/precomp.md) |
| get\_depe\_label\_PRECONJ\_str\(\) | [PRECONJ](../../../../definitions/dependency-labels/preconj.md) |
| get\_depe\_label\_PREDET\_str\(\) | [PREDET](../../../../definitions/dependency-labels/predet.md) |
| get\_depe\_label\_PREF\_str\(\) | [PREF](../../../../definitions/dependency-labels/pref.md) |
| get\_depe\_label\_PREP\_str\(\) | [PREP](../../../../definitions/dependency-labels/prep.md) |
| get\_depe\_label\_PRONL\_str\(\) | [PRONL](../../../../definitions/dependency-labels/pronl.md) |
| get\_depe\_label\_PRT\_str\(\) | [PRT](../../../../definitions/dependency-labels/prt.md) |
| get\_depe\_label\_PS\_str\(\) | [PS](../../../../definitions/dependency-labels/ps.md) |
| get\_depe\_label\_QUANTMOD\_str\(\) | [QUANTMOD](../../../../definitions/dependency-labels/quantmod.md) |
| get\_depe\_label\_RCMOD\_str\(\) | [RCMOD](../../../../definitions/dependency-labels/rcmod.md) |
| get\_depe\_label\_RCMODREL\_str\(\) | [RCMODREL](../../../../definitions/dependency-labels/rcmodrel.md) |
| get\_depe\_label\_RDROP\_str\(\) | [RDROP](../../../../definitions/dependency-labels/rdrop.md) |
| get\_depe\_label\_REF\_str\(\) | [REF](../../../../definitions/dependency-labels/ref.md) |
| get\_depe\_label\_REMNANT\_str\(\) | [REMNANT](../../../../definitions/dependency-labels/remnant.md) |
| get\_depe\_label\_REPARANDUM\_str\(\) | [REPARANDUM](../../../../definitions/dependency-labels/reparandum.md) |
| get\_depe\_label\_ROOT\_str\(\) | [ROOT](../../../../definitions/dependency-labels/root.md) |
| get\_depe\_label\_SNUM\_str\(\) | [SNUM](../../../../definitions/dependency-labels/snum.md) |
| get\_depe\_label\_SUFF\_str\(\) | [SUFF](../../../../definitions/dependency-labels/suff.md) |
| get\_depe\_label\_TMOD\_str\(\) | [TMOD](../../../../definitions/dependency-labels/tmod.md) |
| get\_depe\_label\_TOPIC\_str\(\) | [TOPIC](../../../../definitions/dependency-labels/topic.md) |
| get\_depe\_label\_VMOD\_str\(\) | [VMOD](../../../../definitions/dependency-labels/vmod.md) |
| get\_depe\_label\_VOCATIVE\_str\(\) | [VOCATIVE](../../../../definitions/dependency-labels/vocative.md) |
| get\_depe\_label\_XCOMP\_str\(\) | [XCOMP](../../../../definitions/dependency-labels/xcomp.md) |
| get\_depe\_label\_SUFFIX\_str\(\) | [SUFFIX](../../../../definitions/dependency-labels/suffix.md) |
| get\_depe\_label\_TITLE\_str\(\) | [TITLE](../../../../definitions/dependency-labels/title.md) |
| get\_depe\_label\_ADVPHMOD\_str\(\) | [ADVPHMOD](../../../../definitions/dependency-labels/advphmod.md) |
| get\_depe\_label\_AUXCAUS\_str\(\) | [AUXCAUS](../../../../definitions/dependency-labels/auxcaus.md) |
| get\_depe\_label\_AUXVV\_str\(\) | [AUXVV](../../../../definitions/dependency-labels/auxvv.md) |
| get\_depe\_label\_DTMOD\_str\(\) | [DTMOD](../../../../definitions/dependency-labels/dtmod.md) |
| get\_depe\_label\_FOREIGN\_str\(\) | [FOREIGN](../../../../definitions/dependency-labels/foreign.md) |
| get\_depe\_label\_KW\_str\(\) | [KW](../../../../definitions/dependency-labels/kw.md) |
| get\_depe\_label\_LIST\_str\(\) | [LIST](../../../../definitions/dependency-labels/list.md) |
| get\_depe\_label\_NOMC\_str\(\) | [NOMC](../../../../definitions/dependency-labels/nomc.md) |
| get\_depe\_label\_NOMCSUBJ\_str\(\) | [NOMCSUBJ](../../../../definitions/dependency-labels/nomcsubj.md) |
| get\_depe\_label\_NOMCSUBJPASS\_str\(\) | [NOMCSUBJPASS](../../../../definitions/dependency-labels/nomcsubjpass.md) |
| get\_depe\_label\_NUMC\_str\(\) | [NUMC](../../../../definitions/dependency-labels/numc.md) |
| get\_depe\_label\_COP\_str\(\) | [COP](../../../../definitions/dependency-labels/cop.md) |
| get\_depe\_label\_DISLOCATED\_str\(\) | [DISLOCATED](../../../../definitions/dependency-labels/dislocated.md) |

