# Halbaddierer
inputs: $i_a$ $i_b$

outputs: $o_1$ $o_c$

$o_1 = i_a \oplus i_b$

$o_c = i_a \land i_b$

# Volladdierer
inputs: $i_a$ $i_b$ $i_c$

outputs: $o_1$ $o_c$

$o_1 = (i_a \veebar i_b \veebar i_c) \lor (i_a \land i_b \land i_c)$

$o_c = (i_a \land i_b) \lor (i_b \land i_c) \lor (i_a \land i_c)$
