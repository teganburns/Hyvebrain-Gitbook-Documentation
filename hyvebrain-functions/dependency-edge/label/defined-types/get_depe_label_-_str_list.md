---
description: Alias for functions that retrieve a defined dependency edge label type
---

# get\_depe\_label\_-\_str\_list\(\)

## Parameters

{% tabs %}
{% tab title="Argument" %}
[**`val_vec_int_si`**](../../../variable-types/val_vec_int_si.md)

If no **`val_vec_int_si`** is supplied the argument will default to **`get_sentence_index_list()`**
{% endtab %}

{% tab title="Returns" %}
[**`val_vec_str`**](../../../variable-types/val_vec_str.md)
{% endtab %}

{% tab title="Notes" %}
The content of the return value varies based on the function being called. For example if you were to use the **`get_depe_label_POBJ_str_list()`** function it would return a vector of strings where the [**`val_depe_label`**](../../../variable-types/val_depe_label.md) is a [**POBJ**](../../../../definitions/dependency-labels/pobj.md).
{% endtab %}
{% endtabs %}

## Operation

Iterates through each sentence \([**`val_int_si`**](../../../variable-types/val_int_si.md)\) in the provided vector of sentences \([**`val_vec_int_si`**](../../../variable-types/val_vec_int_si.md)\). Then iterates through each token \([**`val_int_ti`**](../../../variable-types/val_int_ti.md)\) in the aforementioned sentence \([**`val_int_si`**](../../../variable-types/val_int_si.md)\). For each token it will check the dependency edge label \([**`val_depe_label`**](../../../variable-types/val_depe_label.md)\) type. If the dependency edge label type matches the defined type, then the token's string value will be appended to a vector. When there are no more tokens in the sentence and no more sentences in the vector of sentences to iterate though the vector is returned.

{% hint style="success" %}
**Pro-tip**: These functions are almost the same as [**`get_depe_label_-_list()`**](get_depe_label_-_list.md)**\`\`**

Instead of returning a vector of token indexes \([**`val_vec_int_ti`**](../../../variable-types/val_vec_int_ti.md)\) the tokens are represented as a vector of strings \([**`val_vec_str`**](../../../variable-types/val_vec_str.md)\)
{% endhint %}

## Defined Functions

| Function Name                               | Defined Type                                                              |
| :---                                        | :---                                                                      |
| get\_depe\_label\_UNKNOWN_str_list\(\)      | [UNKNOWN](../../../../definitions/dependency-labels/unknown.md)           |
| get\_depe\_label\_ABBREV_str_list\(\)       | [ABBREV](../../../../definitions/dependency-labels/abbrev.md)             |
| get\_depe\_label\_ACOMP_str_list\(\)        | [ACOMP](../../../../definitions/dependency-labels/acomp.md)               |
| get\_depe\_label\_ADVCL_str_list\(\)        | [ADVCL](../../../../definitions/dependency-labels/advcl.md)               |
| get\_depe\_label\_ADVMOD_str_list\(\)       | [ADVMOD](../../../../definitions/dependency-labels/advmod.md)             |
| get\_depe\_label\_AMOD_str_list\(\)         | [AMOD](../../../../definitions/dependency-labels/amod.md)                 |
| get\_depe\_label\_APPOS_str_list\(\)        | [APPOS](../../../../definitions/dependency-labels/appos.md)               |
| get\_depe\_label\_ATTR_str_list\(\)         | [ATTR](../../../../definitions/dependency-labels/attr.md)                 |
| get\_depe\_label\_AUX_str_list\(\)          | [AUX](../../../../definitions/dependency-labels/aux.md)                   |
| get\_depe\_label\_AUXPASS_str_list\(\)      | [AUXPASS](../../../../definitions/dependency-labels/auxpass.md)           |
| get\_depe\_label\_CC_str_list\(\)           | [CC](../../../../definitions/dependency-labels/cc.md)                     |
| get\_depe\_label\_CCOMP_str_list\(\)        | [CCOMP](../../../../definitions/dependency-labels/ccomp.md)               |
| get\_depe\_label\_CONJ_str_list\(\)         | [CONJ](../../../../definitions/dependency-labels/conj.md)                 |
| get\_depe\_label\_CSUBJ_str_list\(\)        | [CSUBJ](../../../../definitions/dependency-labels/csubj.md)               |
| get\_depe\_label\_CSUBJPASS_str_list\(\)    | [CSUBJPASS](../../../../definitions/dependency-labels/csubjpass.md)       |
| get\_depe\_label\_DEP_str_list\(\)          | [DEP](../../../../definitions/dependency-labels/dep.md)                   |
| get\_depe\_label\_DET_str_list\(\)          | [DET](../../../../definitions/dependency-labels/det.md)                   |
| get\_depe\_label\_DISCOURSE_str_list\(\)    | [DISCOURSE](../../../../definitions/dependency-labels/discourse.md)       |
| get\_depe\_label\_DOBJ_str_list\(\)         | [DOBJ](../../../../definitions/dependency-labels/dobj.md)                 |
| get\_depe\_label\_EXPL_str_list\(\)         | [EXPL](../../../../definitions/dependency-labels/expl.md)                 |
| get\_depe\_label\_GOESWITH_str_list\(\)     | [GOESWITH](../../../../definitions/dependency-labels/goeswith.md)         |
| get\_depe\_label\_IOBJ_str_list\(\)         | [IOBJ](../../../../definitions/dependency-labels/iobj.md)                 |
| get\_depe\_label\_MARK_str_list\(\)         | [MARK](../../../../definitions/dependency-labels/mark.md)                 |
| get\_depe\_label\_MWE_str_list\(\)          | [MWE](../../../../definitions/dependency-labels/mwe.md)                   |
| get\_depe\_label\_MWV_str_list\(\)          | [MWV](../../../../definitions/dependency-labels/mwv.md)                   |
| get\_depe\_label\_NEG_str_list\(\)          | [NEG](../../../../definitions/dependency-labels/neg.md)                   |
| get\_depe\_label\_NN_str_list\(\)           | [NN](../../../../definitions/dependency-labels/nn.md)                     |
| get\_depe\_label\_NPADVMOD_str_list\(\)     | [NPADVMOD](../../../../definitions/dependency-labels/npadvmod.md)         |
| get\_depe\_label\_NSUBJ_str_list\(\)        | [NSUBJ](../../../../definitions/dependency-labels/nsubj.md)               |
| get\_depe\_label\_NSUBJPASS_str_list\(\)    | [NSUBJPASS](../../../../definitions/dependency-labels/nsubjpass.md)       |
| get\_depe\_label\_NUM_str_list\(\)          | [NUM](../../../../definitions/dependency-labels/num.md)                   |
| get\_depe\_label\_NUMBER_str_list\(\)       | [NUMBER](../../../../definitions/dependency-labels/number.md)             |
| get\_depe\_label\_P_str_list\(\)            | [P](../../../../definitions/dependency-labels/p.md)                       |
| get\_depe\_label\_PARATAXIS_str_list\(\)    | [PARATAXIS](../../../../definitions/dependency-labels/parataxis.md)       |
| get\_depe\_label\_PARTMOD_str_list\(\)      | [PARTMOD](../../../../definitions/dependency-labels/partmod.md)           |
| get\_depe\_label\_PCOMP_str_list\(\)        | [PCOMP](../../../../definitions/dependency-labels/pcomp.md)               |
| get\_depe\_label\_POBJ_str_list\(\)         | [POBJ](../../../../definitions/dependency-labels/pobj.md)                 |
| get\_depe\_label\_POSS_str_list\(\)         | [POSS](../../../../definitions/dependency-labels/poss.md)                 |
| get\_depe\_label\_POSTNEG_str_list\(\)      | [POSTNEG](../../../../definitions/dependency-labels/postneg.md)           |
| get\_depe\_label\_PRECOMP_str_list\(\)      | [PRECOMP](../../../../definitions/dependency-labels/precomp.md)           |
| get\_depe\_label\_PRECONJ_str_list\(\)      | [PRECONJ](../../../../definitions/dependency-labels/preconj.md)           |
| get\_depe\_label\_PREDET_str_list\(\)       | [PREDET](../../../../definitions/dependency-labels/predet.md)             |
| get\_depe\_label\_PREF_str_list\(\)         | [PREF](../../../../definitions/dependency-labels/pref.md)                 |
| get\_depe\_label\_PREP_str_list\(\)         | [PREP](../../../../definitions/dependency-labels/prep.md)                 |
| get\_depe\_label\_PRONL_str_list\(\)        | [PRONL](../../../../definitions/dependency-labels/pronl.md)               |
| get\_depe\_label\_PRT_str_list\(\)          | [PRT](../../../../definitions/dependency-labels/prt.md)                   |
| get\_depe\_label\_PS_str_list\(\)           | [PS](../../../../definitions/dependency-labels/ps.md)                     |
| get\_depe\_label\_QUANTMOD_str_list\(\)     | [QUANTMOD](../../../../definitions/dependency-labels/quantmod.md)         |
| get\_depe\_label\_RCMOD_str_list\(\)        | [RCMOD](../../../../definitions/dependency-labels/rcmod.md)               |
| get\_depe\_label\_RCMODREL_str_list\(\)     | [RCMODREL](../../../../definitions/dependency-labels/rcmodrel.md)         |
| get\_depe\_label\_RDROP_str_list\(\)        | [RDROP](../../../../definitions/dependency-labels/rdrop.md)               |
| get\_depe\_label\_REF_str_list\(\)          | [REF](../../../../definitions/dependency-labels/ref.md)                   |
| get\_depe\_label\_REMNANT_str_list\(\)      | [REMNANT](../../../../definitions/dependency-labels/remnant.md)           |
| get\_depe\_label\_REPARANDUM_str_list\(\)   | [REPARANDUM](../../../../definitions/dependency-labels/reparandum.md)     |
| get\_depe\_label\_ROOT_str_list\(\)         | [ROOT](../../../../definitions/dependency-labels/root.md)                 |
| get\_depe\_label\_SNUM_str_list\(\)         | [SNUM](../../../../definitions/dependency-labels/snum.md)                 |
| get\_depe\_label\_SUFF_str_list\(\)         | [SUFF](../../../../definitions/dependency-labels/suff.md)                 |
| get\_depe\_label\_TMOD_str_list\(\)         | [TMOD](../../../../definitions/dependency-labels/tmod.md)                 |
| get\_depe\_label\_TOPIC_str_list\(\)        | [TOPIC](../../../../definitions/dependency-labels/topic.md)               |
| get\_depe\_label\_VMOD_str_list\(\)         | [VMOD](../../../../definitions/dependency-labels/vmod.md)                 |
| get\_depe\_label\_VOCATIVE_str_list\(\)     | [VOCATIVE](../../../../definitions/dependency-labels/vocative.md)         |
| get\_depe\_label\_XCOMP_str_list\(\)        | [XCOMP](../../../../definitions/dependency-labels/xcomp.md)               |
| get\_depe\_label\_SUFFIX_str_list\(\)       | [SUFFIX](../../../../definitions/dependency-labels/suffix.md)             |
| get\_depe\_label\_TITLE_str_list\(\)        | [TITLE](../../../../definitions/dependency-labels/title.md)               |
| get\_depe\_label\_ADVPHMOD_str_list\(\)     | [ADVPHMOD](../../../../definitions/dependency-labels/advphmod.md)         |
| get\_depe\_label\_AUXCAUS_str_list\(\)      | [AUXCAUS](../../../../definitions/dependency-labels/auxcaus.md)           |
| get\_depe\_label\_AUXVV_str_list\(\)        | [AUXVV](../../../../definitions/dependency-labels/auxvv.md)               |
| get\_depe\_label\_DTMOD_str_list\(\)        | [DTMOD](../../../../definitions/dependency-labels/dtmod.md)               |
| get\_depe\_label\_FOREIGN_str_list\(\)      | [FOREIGN](../../../../definitions/dependency-labels/foreign.md)           |
| get\_depe\_label\_KW_str_list\(\)           | [KW](../../../../definitions/dependency-labels/kw.md)                     |
| get\_depe\_label\_LIST_str_list\(\)         | [LIST](../../../../definitions/dependency-labels/list.md)                 |
| get\_depe\_label\_NOMC_str_list\(\)         | [NOMC](../../../../definitions/dependency-labels/nomc.md)                 |
| get\_depe\_label\_NOMCSUBJ_str_list\(\)     | [NOMCSUBJ](../../../../definitions/dependency-labels/nomcsubj.md)         |
| get\_depe\_label\_NOMCSUBJPASS_str_list\(\) | [NOMCSUBJPASS](../../../../definitions/dependency-labels/nomcsubjpass.md) |
| get\_depe\_label\_NUMC_str_list\(\)         | [NUMC](../../../../definitions/dependency-labels/numc.md)                 |
| get\_depe\_label\_COP_str_list\(\)          | [COP](../../../../definitions/dependency-labels/cop.md)                   |
| get\_depe\_label\_DISLOCATED_str_list\(\)   | [DISLOCATED](../../../../definitions/dependency-labels/dislocated.md)     |



