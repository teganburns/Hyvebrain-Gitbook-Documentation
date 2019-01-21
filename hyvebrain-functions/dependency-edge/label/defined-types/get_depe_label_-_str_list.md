---
description: Alias for functions that retrieve a defined dependency edge label type
---

# get\_depe\_label\_-\_str\_list\(\)

## Parameters

{% tabs %}
{% tab title="Argument" %}
[`val_vec_int_si`](../../../variable-types/val_vec_int_si.md)

If no `val_vec_int_si` is supplied the argument will default to `get_sentence_index_list()`
{% endtab %}

{% tab title="Returns" %}
[`val_vec_str`](../../../variable-types/val_vec_str.md)
{% endtab %}

{% tab title="Notes" %}
The content of the return value varies based on the function being called. For example if you were to use the `get_depe_label_POBJ_str_list()` function it would return a vector of strings where the [`val_depe_label`](../../../variable-types/val_depe_label.md) is a [**POBJ**](../../../../definitions/dependency-labels/pobj.md).
{% endtab %}
{% endtabs %}

## Operation

Iterates through each sentence \([`val_int_si`](../../../variable-types/val_int_si.md)\) in the provided vector of sentences \([`val_vec_int_si`](../../../variable-types/val_vec_int_si.md)\). Then iterates through each token \([`val_int_ti`](../../../variable-types/val_int_ti.md)\) in the aforementioned sentence \([`val_int_si`](../../../variable-types/val_int_si.md)\). For each token it will check the dependency edge label \([`val_depe_label`](../../../variable-types/val_depe_label.md)\) type. If the dependency edge label type matches the defined type, then the token's string value will be appended to a vector. When there are no more tokens in the sentence and no more sentences in the vector of sentences to iterate though the vector is returned.

{% hint style="success" %}
**Pro-tip**: These functions are almost the same as [`get_depe_label_-_list()`](get_depe_label_-_list.md)

Instead of returning a vector of token indexes \([`val_vec_int_ti`](../../../variable-types/val_vec_int_ti.md)\) the tokens are represented as a vector of strings \([`val_vec_str`](../../../variable-types/val_vec_str.md)\)
{% endhint %}

## Defined Functions

| Function Name | Defined Type |
| :--- | :--- |
| get\_depe\_label\_UNKNOWN\_str\_list\(\) | [UNKNOWN](../../../../definitions/dependency-labels/unknown.md) |
| get\_depe\_label\_ABBREV\_str\_list\(\) | [ABBREV](../../../../definitions/dependency-labels/abbrev.md) |
| get\_depe\_label\_ACOMP\_str\_list\(\) | [ACOMP](../../../../definitions/dependency-labels/acomp.md) |
| get\_depe\_label\_ADVCL\_str\_list\(\) | [ADVCL](../../../../definitions/dependency-labels/advcl.md) |
| get\_depe\_label\_ADVMOD\_str\_list\(\) | [ADVMOD](../../../../definitions/dependency-labels/advmod.md) |
| get\_depe\_label\_AMOD\_str\_list\(\) | [AMOD](../../../../definitions/dependency-labels/amod.md) |
| get\_depe\_label\_APPOS\_str\_list\(\) | [APPOS](../../../../definitions/dependency-labels/appos.md) |
| get\_depe\_label\_ATTR\_str\_list\(\) | [ATTR](../../../../definitions/dependency-labels/attr.md) |
| get\_depe\_label\_AUX\_str\_list\(\) | [AUX](../../../../definitions/dependency-labels/aux.md) |
| get\_depe\_label\_AUXPASS\_str\_list\(\) | [AUXPASS](../../../../definitions/dependency-labels/auxpass.md) |
| get\_depe\_label\_CC\_str\_list\(\) | [CC](../../../../definitions/dependency-labels/cc.md) |
| get\_depe\_label\_CCOMP\_str\_list\(\) | [CCOMP](../../../../definitions/dependency-labels/ccomp.md) |
| get\_depe\_label\_CONJ\_str\_list\(\) | [CONJ](../../../../definitions/dependency-labels/conj.md) |
| get\_depe\_label\_CSUBJ\_str\_list\(\) | [CSUBJ](../../../../definitions/dependency-labels/csubj.md) |
| get\_depe\_label\_CSUBJPASS\_str\_list\(\) | [CSUBJPASS](../../../../definitions/dependency-labels/csubjpass.md) |
| get\_depe\_label\_DEP\_str\_list\(\) | [DEP](../../../../definitions/dependency-labels/dep.md) |
| get\_depe\_label\_DET\_str\_list\(\) | [DET](../../../../definitions/dependency-labels/det.md) |
| get\_depe\_label\_DISCOURSE\_str\_list\(\) | [DISCOURSE](../../../../definitions/dependency-labels/discourse.md) |
| get\_depe\_label\_DOBJ\_str\_list\(\) | [DOBJ](../../../../definitions/dependency-labels/dobj.md) |
| get\_depe\_label\_EXPL\_str\_list\(\) | [EXPL](../../../../definitions/dependency-labels/expl.md) |
| get\_depe\_label\_GOESWITH\_str\_list\(\) | [GOESWITH](../../../../definitions/dependency-labels/goeswith.md) |
| get\_depe\_label\_IOBJ\_str\_list\(\) | [IOBJ](../../../../definitions/dependency-labels/iobj.md) |
| get\_depe\_label\_MARK\_str\_list\(\) | [MARK](../../../../definitions/dependency-labels/mark.md) |
| get\_depe\_label\_MWE\_str\_list\(\) | [MWE](../../../../definitions/dependency-labels/mwe.md) |
| get\_depe\_label\_MWV\_str\_list\(\) | [MWV](../../../../definitions/dependency-labels/mwv.md) |
| get\_depe\_label\_NEG\_str\_list\(\) | [NEG](../../../../definitions/dependency-labels/neg.md) |
| get\_depe\_label\_NN\_str\_list\(\) | [NN](../../../../definitions/dependency-labels/nn.md) |
| get\_depe\_label\_NPADVMOD\_str\_list\(\) | [NPADVMOD](../../../../definitions/dependency-labels/npadvmod.md) |
| get\_depe\_label\_NSUBJ\_str\_list\(\) | [NSUBJ](../../../../definitions/dependency-labels/nsubj.md) |
| get\_depe\_label\_NSUBJPASS\_str\_list\(\) | [NSUBJPASS](../../../../definitions/dependency-labels/nsubjpass.md) |
| get\_depe\_label\_NUM\_str\_list\(\) | [NUM](../../../../definitions/dependency-labels/num.md) |
| get\_depe\_label\_NUMBER\_str\_list\(\) | [NUMBER](../../../../definitions/dependency-labels/number.md) |
| get\_depe\_label\_P\_str\_list\(\) | [P](../../../../definitions/dependency-labels/p.md) |
| get\_depe\_label\_PARATAXIS\_str\_list\(\) | [PARATAXIS](../../../../definitions/dependency-labels/parataxis.md) |
| get\_depe\_label\_PARTMOD\_str\_list\(\) | [PARTMOD](../../../../definitions/dependency-labels/partmod.md) |
| get\_depe\_label\_PCOMP\_str\_list\(\) | [PCOMP](../../../../definitions/dependency-labels/pcomp.md) |
| get\_depe\_label\_POBJ\_str\_list\(\) | [POBJ](../../../../definitions/dependency-labels/pobj.md) |
| get\_depe\_label\_POSS\_str\_list\(\) | [POSS](../../../../definitions/dependency-labels/poss.md) |
| get\_depe\_label\_POSTNEG\_str\_list\(\) | [POSTNEG](../../../../definitions/dependency-labels/postneg.md) |
| get\_depe\_label\_PRECOMP\_str\_list\(\) | [PRECOMP](../../../../definitions/dependency-labels/precomp.md) |
| get\_depe\_label\_PRECONJ\_str\_list\(\) | [PRECONJ](../../../../definitions/dependency-labels/preconj.md) |
| get\_depe\_label\_PREDET\_str\_list\(\) | [PREDET](../../../../definitions/dependency-labels/predet.md) |
| get\_depe\_label\_PREF\_str\_list\(\) | [PREF](../../../../definitions/dependency-labels/pref.md) |
| get\_depe\_label\_PREP\_str\_list\(\) | [PREP](../../../../definitions/dependency-labels/prep.md) |
| get\_depe\_label\_PRONL\_str\_list\(\) | [PRONL](../../../../definitions/dependency-labels/pronl.md) |
| get\_depe\_label\_PRT\_str\_list\(\) | [PRT](../../../../definitions/dependency-labels/prt.md) |
| get\_depe\_label\_PS\_str\_list\(\) | [PS](../../../../definitions/dependency-labels/ps.md) |
| get\_depe\_label\_QUANTMOD\_str\_list\(\) | [QUANTMOD](../../../../definitions/dependency-labels/quantmod.md) |
| get\_depe\_label\_RCMOD\_str\_list\(\) | [RCMOD](../../../../definitions/dependency-labels/rcmod.md) |
| get\_depe\_label\_RCMODREL\_str\_list\(\) | [RCMODREL](../../../../definitions/dependency-labels/rcmodrel.md) |
| get\_depe\_label\_RDROP\_str\_list\(\) | [RDROP](../../../../definitions/dependency-labels/rdrop.md) |
| get\_depe\_label\_REF\_str\_list\(\) | [REF](../../../../definitions/dependency-labels/ref.md) |
| get\_depe\_label\_REMNANT\_str\_list\(\) | [REMNANT](../../../../definitions/dependency-labels/remnant.md) |
| get\_depe\_label\_REPARANDUM\_str\_list\(\) | [REPARANDUM](../../../../definitions/dependency-labels/reparandum.md) |
| get\_depe\_label\_ROOT\_str\_list\(\) | [ROOT](../../../../definitions/dependency-labels/root.md) |
| get\_depe\_label\_SNUM\_str\_list\(\) | [SNUM](../../../../definitions/dependency-labels/snum.md) |
| get\_depe\_label\_SUFF\_str\_list\(\) | [SUFF](../../../../definitions/dependency-labels/suff.md) |
| get\_depe\_label\_TMOD\_str\_list\(\) | [TMOD](../../../../definitions/dependency-labels/tmod.md) |
| get\_depe\_label\_TOPIC\_str\_list\(\) | [TOPIC](../../../../definitions/dependency-labels/topic.md) |
| get\_depe\_label\_VMOD\_str\_list\(\) | [VMOD](../../../../definitions/dependency-labels/vmod.md) |
| get\_depe\_label\_VOCATIVE\_str\_list\(\) | [VOCATIVE](../../../../definitions/dependency-labels/vocative.md) |
| get\_depe\_label\_XCOMP\_str\_list\(\) | [XCOMP](../../../../definitions/dependency-labels/xcomp.md) |
| get\_depe\_label\_SUFFIX\_str\_list\(\) | [SUFFIX](../../../../definitions/dependency-labels/suffix.md) |
| get\_depe\_label\_TITLE\_str\_list\(\) | [TITLE](../../../../definitions/dependency-labels/title.md) |
| get\_depe\_label\_ADVPHMOD\_str\_list\(\) | [ADVPHMOD](../../../../definitions/dependency-labels/advphmod.md) |
| get\_depe\_label\_AUXCAUS\_str\_list\(\) | [AUXCAUS](../../../../definitions/dependency-labels/auxcaus.md) |
| get\_depe\_label\_AUXVV\_str\_list\(\) | [AUXVV](../../../../definitions/dependency-labels/auxvv.md) |
| get\_depe\_label\_DTMOD\_str\_list\(\) | [DTMOD](../../../../definitions/dependency-labels/dtmod.md) |
| get\_depe\_label\_FOREIGN\_str\_list\(\) | [FOREIGN](../../../../definitions/dependency-labels/foreign.md) |
| get\_depe\_label\_KW\_str\_list\(\) | [KW](../../../../definitions/dependency-labels/kw.md) |
| get\_depe\_label\_LIST\_str\_list\(\) | [LIST](../../../../definitions/dependency-labels/list.md) |
| get\_depe\_label\_NOMC\_str\_list\(\) | [NOMC](../../../../definitions/dependency-labels/nomc.md) |
| get\_depe\_label\_NOMCSUBJ\_str\_list\(\) | [NOMCSUBJ](../../../../definitions/dependency-labels/nomcsubj.md) |
| get\_depe\_label\_NOMCSUBJPASS\_str\_list\(\) | [NOMCSUBJPASS](../../../../definitions/dependency-labels/nomcsubjpass.md) |
| get\_depe\_label\_NUMC\_str\_list\(\) | [NUMC](../../../../definitions/dependency-labels/numc.md) |
| get\_depe\_label\_COP\_str\_list\(\) | [COP](../../../../definitions/dependency-labels/cop.md) |
| get\_depe\_label\_DISLOCATED\_str\_list\(\) | [DISLOCATED](../../../../definitions/dependency-labels/dislocated.md) |

