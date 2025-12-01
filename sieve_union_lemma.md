# Proof for sieve_union_lemma
An error occurred while trying to save your proof in PVS.
If the problem persists, please report an issue on [github](https://github.com/nasa/vscode-pvs/issues) or on the [PVS group](https://groups.google.com/g/pvs-group), we will look into it.

## Your proof attempt
Don't panic, your proof attempt for sieve_union_lemma is not lost.<br>
VSCode-PVS saved your proof attempt, and you can restore it from the Proof Explorer menu **...** -> **Restore Proof**<br>

If everything else fails, below you can find the complete proof script, which you can paste in the prover terminal to repeat the proof:
```lisp
(measure-induct+ "length(pl)" pl)(skeep)(expand "sieve_union" 1)(lift-if)(split)(flatten)(expand "list_prod_l2" 1)(expand "length" -1)(expand "list_prod_l2" 1)(lift-if)(split)(flatten)(expand "list_prod" 1)(expand "list_prod" 1)(assert)(typepred "card_sl(difference_sl(list_less(m), list_sieve0(m, car(x!1), car(rl))))")(lemma "difference_l2s")(inst?)(replaces -1)(lemma "card_diff_subset")(inst?)(prop)(typepred "card(difference(list2set(list_less(m)), list2set(list_sieve0(m, car(x!1), car(rl)))))")(replaces -1)(replaces -1)(expand "list_sieve0" -1 2)(rewrite "union_l2s")(lemma "card_disj_union")(inst?)(prop)(replaces -1)(typepred "card_sl(list_less(m))")(typepred "card(list2set(list_less(m)))")(replaces -1)(replaces -1 :dir rl)(typepred "card_sl(list_sieve_aux(m, car(x!1), 0))")(typepred "card(list2set(list_sieve_aux(m, car(x!1), 0)))")(replaces -1)(replaces -1 :dir rl)(typepred "card_sl(list_sieve(m, car(x!1), car(rl)))")(typepred "card(list2set(list_sieve(m, car(x!1), car(rl))))")(replaces -1)(replaces -1 :dir rl)(replaces -1)(rewrite "card_sl_list_less")(postpone)(postpone)(postpone)(postpone)(postpone)(postpone)(postpone)(postpone)(postpone)(postpone)(postpone)(postpone)(postpone)(postpone)
```