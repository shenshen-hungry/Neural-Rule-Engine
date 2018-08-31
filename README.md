# Rules Used in Neural Rule Engine
We release the rules served for Relation Classification (SemEval-2010 Task 8) in the paper:

Shen Li, Hengru Xu, Zhengdong Lu, <a href="https://arxiv.org/abs/1808.10326"><em>Generalize Symbolic Knowledge With Neural Rule Engine</em></a>

Each rule is defined as: [positive]@@[negative]

where [positive] means something that a case must have if the case is matched by the rule, and [negative] means the case mustn't have.

For example, given a case and a rule:

Case: The \<e1\>island\</e1\> was farmed for \<e2\>oats\</e2\> and barley until 1796 when the owner mandated that oak and alder trees be planted.

Rule: island.\*\</e1\>.\*farmed for.\*\<e2\>@@\<e2\>(year|profit).\*\</e2\>

since the case has "island.\*\</e1\>.\*farmed for.\*\<e2\>" and hasn't "\<e2\>(year|profit).\*\</e2\>", the case is matched by the rule.
