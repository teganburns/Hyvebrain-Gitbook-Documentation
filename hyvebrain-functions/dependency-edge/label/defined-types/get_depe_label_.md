---
description: Alias for functions that retrieve a defined dependency edge label type
---

# get\_depe\_label\_-\(\)

## Parameters

{% tabs %}
{% tab title="Argument" %}
[**`val_int_si`**](../../../variable-types/val_int_si.md)

If no **`val_int_si`** is supplied the argument will default to **`get_current_sentence_index()`**
{% endtab %}

{% tab title="Returns" %}
\*\*\*\*[**`val_vec_int_ti`**](../../../variable-types/val_vec_int_ti.md)
{% endtab %}

{% tab title="Notes" %}
The content of the return value varies based on the function being called. For example if you were to use the **`get_depe_label_POBJ()`** function it would return a vector of token indexes where the [**`val_depe_label`**](../../../variable-types/val_depe_label.md) is a [**POBJ**](../../../../definitions/dependency-labels/pobj.md).
{% endtab %}
{% endtabs %}

## Operation

Iterates through each token \([**`val_int_ti`**](https://docs.hyvebrain.com/~/drafts/-LUwZHJukv0KMhgvdvUK/primary/hyvebrain-functions/variable-types/val_int_ti)\) in the provided sentence \([**`val_int_si`**](https://docs.hyvebrain.com/~/drafts/-LUwZHJukv0KMhgvdvUK/primary/hyvebrain-functions/variable-types/val_int_si)\). For each token it will check the dependency edge label \([**`val_depe_label`**](../../../variable-types/val_depe_label.md)\) type. If the dependency edge label type matches the defined type the token's index will be appended to a vector. When there are no more tokens in the sentence to iterate though the vector is returned.

## Defined Functions

| Function Name | Defined Type |
| :--- | :--- |
| get\_depe\_label\_UNKNOWN\(\) | [UNKNOWN](../../../../definitions/dependency-labels/unknown.md) |
| get\_depe\_label\_ABBREV\(\) | [ABBREV](../../../../definitions/dependency-labels/abbrev.md) |
| get\_depe\_label\_ACOMP\(\) | [ACOMP](../../../../definitions/dependency-labels/acomp.md) |
| get\_depe\_label\_ADVCL\(\) | [ADVCL](../../../../definitions/dependency-labels/advcl.md) |
| get\_depe\_label\_ADVMOD\(\) | [ADVMOD](../../../../definitions/dependency-labels/advmod.md) |
| get\_depe\_label\_AMOD\(\) | [AMOD](../../../../definitions/dependency-labels/amod.md) |
| get\_depe\_label\_APPOS\(\) | [APPOS](../../../../definitions/dependency-labels/appos.md) |
| get\_depe\_label\_ATTR\(\) | [ATTR](../../../../definitions/dependency-labels/attr.md) |
| get\_depe\_label\_AUX\(\) | [AUX](../../../../definitions/dependency-labels/aux.md) |
| get\_depe\_label\_AUXPASS\(\) | [AUXPASS](../../../../definitions/dependency-labels/auxpass.md) |
| get\_depe\_label\_CC\(\) | [CC](../../../../definitions/dependency-labels/cc.md) |
| get\_depe\_label\_CCOMP\(\) | [CCOMP](../../../../definitions/dependency-labels/ccomp.md) |
| get\_depe\_label\_CONJ\(\) | [CONJ](../../../../definitions/dependency-labels/conj.md) |
| get\_depe\_label\_CSUBJ\(\) | [CSUBJ](../../../../definitions/dependency-labels/csubj.md) |
| get\_depe\_label\_CSUBJPASS\(\) | [CSUBJPASS](../../../../definitions/dependency-labels/csubjpass.md) |
| get\_depe\_label\_DEP\(\) | [DEP](../../../../definitions/dependency-labels/dep.md) |
| get\_depe\_label\_DET\(\) | [DET](../../../../definitions/dependency-labels/det.md) |
| get\_depe\_label\_DISCOURSE\(\) | [DISCOURSE](../../../../definitions/dependency-labels/discourse.md) |
| get\_depe\_label\_DOBJ\(\) | [DOBJ](../../../../definitions/dependency-labels/dobj.md) |
| get\_depe\_label\_EXPL\(\) | [EXPL](../../../../definitions/dependency-labels/expl.md) |
| get\_depe\_label\_GOESWITH\(\) | [GOESWITH](../../../../definitions/dependency-labels/goeswith.md) |
| get\_depe\_label\_IOBJ\(\) | [IOBJ](../../../../definitions/dependency-labels/iobj.md) |
| get\_depe\_label\_MARK\(\) | [MARK](../../../../definitions/dependency-labels/mark.md) |
| get\_depe\_label\_MWE\(\) | [MWE](../../../../definitions/dependency-labels/mwe.md) |
| get\_depe\_label\_MWV\(\) | [MWV](../../../../definitions/dependency-labels/mwv.md) |
| get\_depe\_label\_NEG\(\) | [NEG](../../../../definitions/dependency-labels/neg.md) |
| get\_depe\_label\_NN\(\) | [NN](../../../../definitions/dependency-labels/nn.md) |
| get\_depe\_label\_NPADVMOD\(\) | [NPADVMOD](../../../../definitions/dependency-labels/npadvmod.md) |
| get\_depe\_label\_NSUBJ\(\) | [NSUBJ](../../../../definitions/dependency-labels/nsubj.md) |
| get\_depe\_label\_NSUBJPASS\(\) | [NSUBJPASS](../../../../definitions/dependency-labels/nsubjpass.md) |
| get\_depe\_label\_NUM\(\) | [NUM](../../../../definitions/dependency-labels/num.md) |
| get\_depe\_label\_NUMBER\(\) | [NUMBER](../../../../definitions/dependency-labels/number.md) |
| get\_depe\_label\_P\(\) | [P](../../../../definitions/dependency-labels/p.md) |
| get\_depe\_label\_PARATAXIS\(\) | [PARATAXIS](../../../../definitions/dependency-labels/parataxis.md) |
| get\_depe\_label\_PARTMOD\(\) | [PARTMOD](../../../../definitions/dependency-labels/partmod.md) |
| get\_depe\_label\_PCOMP\(\) | [PCOMP](../../../../definitions/dependency-labels/pcomp.md) |
| get\_depe\_label\_POBJ\(\) | [POBJ](../../../../definitions/dependency-labels/pobj.md) |
| get\_depe\_label\_POSS\(\) | [POSS](../../../../definitions/dependency-labels/poss.md) |
| get\_depe\_label\_POSTNEG\(\) | [POSTNEG](../../../../definitions/dependency-labels/postneg.md) |
| get\_depe\_label\_PRECOMP\(\) | [PRECOMP](../../../../definitions/dependency-labels/precomp.md) |
| get\_depe\_label\_PRECONJ\(\) | [PRECONJ](../../../../definitions/dependency-labels/preconj.md) |
| get\_depe\_label\_PREDET\(\) | [PREDET](../../../../definitions/dependency-labels/predet.md) |
| get\_depe\_label\_PREF\(\) | [PREF](../../../../definitions/dependency-labels/pref.md) |
| get\_depe\_label\_PREP\(\) | [PREP](../../../../definitions/dependency-labels/prep.md) |
| get\_depe\_label\_PRONL\(\) | [PRONL](../../../../definitions/dependency-labels/pronl.md) |
| get\_depe\_label\_PRT\(\) | [PRT](../../../../definitions/dependency-labels/prt.md) |
| get\_depe\_label\_PS\(\) | [PS](../../../../definitions/dependency-labels/ps.md) |
| get\_depe\_label\_QUANTMOD\(\) | [QUANTMOD](../../../../definitions/dependency-labels/quantmod.md) |
| get\_depe\_label\_RCMOD\(\) | [RCMOD](../../../../definitions/dependency-labels/rcmod.md) |
| get\_depe\_label\_RCMODREL\(\) | [RCMODREL](../../../../definitions/dependency-labels/rcmodrel.md) |
| get\_depe\_label\_RDROP\(\) | [RDROP](../../../../definitions/dependency-labels/rdrop.md) |
| get\_depe\_label\_REF\(\) | [REF](../../../../definitions/dependency-labels/ref.md) |
| get\_depe\_label\_REMNANT\(\) | [REMNANT](../../../../definitions/dependency-labels/remnant.md) |
| get\_depe\_label\_REPARANDUM\(\) | [REPARANDUM](../../../../definitions/dependency-labels/reparandum.md) |
| get\_depe\_label\_ROOT\(\) | [ROOT](../../../../definitions/dependency-labels/root.md) |
| get\_depe\_label\_SNUM\(\) | [SNUM](../../../../definitions/dependency-labels/snum.md) |
| get\_depe\_label\_SUFF\(\) | [SUFF](../../../../definitions/dependency-labels/suff.md) |
| get\_depe\_label\_TMOD\(\) | [TMOD](../../../../definitions/dependency-labels/tmod.md) |
| get\_depe\_label\_TOPIC\(\) | [TOPIC](../../../../definitions/dependency-labels/topic.md) |
| get\_depe\_label\_VMOD\(\) | [VMOD](../../../../definitions/dependency-labels/vmod.md) |
| get\_depe\_label\_VOCATIVE\(\) | [VOCATIVE](../../../../definitions/dependency-labels/vocative.md) |
| get\_depe\_label\_XCOMP\(\) | [XCOMP](../../../../definitions/dependency-labels/xcomp.md) |
| get\_depe\_label\_SUFFIX\(\) | [SUFFIX](../../../../definitions/dependency-labels/suffix.md) |
| get\_depe\_label\_TITLE\(\) | [TITLE](../../../../definitions/dependency-labels/title.md) |
| get\_depe\_label\_ADVPHMOD\(\) | [ADVPHMOD](../../../../definitions/dependency-labels/advphmod.md) |
| get\_depe\_label\_AUXCAUS\(\) | [AUXCAUS](../../../../definitions/dependency-labels/auxcaus.md) |
| get\_depe\_label\_AUXVV\(\) | [AUXVV](../../../../definitions/dependency-labels/auxvv.md) |
| get\_depe\_label\_DTMOD\(\) | [DTMOD](../../../../definitions/dependency-labels/dtmod.md) |
| get\_depe\_label\_FOREIGN\(\) | [FOREIGN](../../../../definitions/dependency-labels/foreign.md) |
| get\_depe\_label\_KW\(\) | [KW](../../../../definitions/dependency-labels/kw.md) |
| get\_depe\_label\_LIST\(\) | [LIST](../../../../definitions/dependency-labels/list.md) |
| get\_depe\_label\_NOMC\(\) | [NOMC](../../../../definitions/dependency-labels/nomc.md) |
| get\_depe\_label\_NOMCSUBJ\(\) | [NOMCSUBJ](../../../../definitions/dependency-labels/nomcsubj.md) |
| get\_depe\_label\_NOMCSUBJPASS\(\) | [NOMCSUBJPASS](../../../../definitions/dependency-labels/nomcsubjpass.md) |
| get\_depe\_label\_NUMC\(\) | [NUMC](../../../../definitions/dependency-labels/numc.md) |
| get\_depe\_label\_COP\(\) | [COP](../../../../definitions/dependency-labels/cop.md) |
| get\_depe\_label\_DISLOCATED\(\) | [DISLOCATED](../../../../definitions/dependency-labels/dislocated.md) |



