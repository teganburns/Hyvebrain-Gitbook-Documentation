# val\_int\_si

## Synopsis

**val\_int\_si** is an **Integer** that represents the current sentence index.

**val\_int\_si** is **null** until initialized in a function that either returns **val\_int\_ti** or takes **val\_int\_ti** as an argument.

The sentence index is the position \(aka. index\) in which a sentence occurs in the text content . If we take the first paragraph from the Wikipedia article on Turing test, referenced below, we can see that there are six sentences in the paragraph.

> The Turing test, developed by Alan Turing in 1950, is a test of a machine's ability to exhibit intelligent behavior equivalent to, or indistinguishable from, that of a human. 
>
> Turing proposed that a human evaluator would judge natural language conversations between a human and a machine designed to generate human-like responses.
>
>  The evaluator would be aware that one of the two partners in conversation is a machine, and all participants would be separated from one another. 
>
> The conversation would be limited to a text-only channel such as a computer keyboard and screen so the result would not depend on the machine's ability to render words as speech. 
>
> If the evaluator cannot reliably tell the machine from the human, the machine is said to have passed the test. 
>
> The test results do not depend on the machine's ability to give correct answers to questions, only how closely its answers resemble those a human would give.

{% hint style="warning" %}
The sentence index \( **val\_int\_si** \) will always starts at zero
{% endhint %}

**val\_int\_si** is a zero indexed array. This means that when counting the sentences you will always start at zero instead of one. To read more about zero indexed arrays see [Zero-based numbering](https://en.wikipedia.org/wiki/Zero-based_numbering).

