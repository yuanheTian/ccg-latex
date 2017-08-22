The commands in the <code>ccg-latex.sty</code> file can be used to typeset Combinatory Categorial Grammar (CCG) derivations.

Example file shows how.

The basic command is <code>\begin{ccg}..\end{ccg}</code>. It typesets
derivations without glosses. 

It has a variant, <code>\begin{ccgg}..\end{ccgg}</code>,
which typesets glosses before the top lines are drawn.

Both are based on <code>\cgex{n}{ders}</code>, which is kept for legacy code, where <code>n</code> is the number of columns,
and <code>ders</code> is the \\ \\-separated lines of at most that many columns.

Basic commands other than above:

<code>\cgf{..}</code> typesets the syntactic category.

<code>\cat{..}</code> typesets the syntactic category. It is an alias of <code>\cgf{..}</code>.

<code>\lf{..}</code> typesets the logical form.

<code>\combx</code> typesets the combinator x in bold Curry and Feys notation.

<code>\cgs{..}{..}</code> typesets a subscripted category.

<code>\cgline{n}{rulename}</code> draws a CCG line across n columns, and indexes it with the rule. 

  Rule names are <code>\cgfa, \cgba, \cgfc, \cgbc</code> etc. Rulename need not be a pre-defined rule name.

<code>\cgres{n}{..}</code> typesets the material in .. across n columns.

<code>\cglines{n}</code> typesets n undecorated lines separated by blanks, which is common practice after lexical assumptions.

<code>\badline{n}{rulename}</code> typesets a line spanning n columns with <code>***</code> in the middle, with rule name at the end.

<code>\mc{n}{text}</code> typesets the text multi-column centered over n columns; useful for foreign language glossing.

<code>\fstars</code> is a forward slash with star modality, i.e. <code>/*</code>. 

<code>\bxs</code> is a backward slash with crossing modality, i.e. <code>\x</code>. 

Defined for all slashes and modalities.
