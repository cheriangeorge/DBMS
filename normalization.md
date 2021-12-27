#### Additional Normal Forms
- ◦ Elementary Key Normal Form (EKNF)
- ◦ Boyce-codd Normal Form (BCNF)
- ◦ Multivalued Dependencies And Fourth Normal Form (4NF)
- ◦ Essential Tuple Normal Form (ETNF)
- ◦ Join Dependencies and Fifth Normal Form (5NF)
- ◦ Sixth Normal Form (6NF)
- ◦ Domain/Key Normal Form (DKNF)


#### 1NF - A relation is in First Normal Form if and only if all underlying domains contain atomic
values only (doesn’t have multivalued attributes (MVA))

#### 2NF - Relation R is in Second Normal Form (2NF) only iff : 
- ◦ R is in 1NF and
- ◦ R contains no Partial Dependency

#### Partial Dependency - 
(Y → A) is a Partial dependency only if
- • Y : Proper subset of Candidate Key
- • A: Non Prime Attribute
A prime attribute of a relation is an attribute that is a part of a candidate key of the relation

#### 3NF - A relational schema R is in 3NF if for every FD X → A associated with R either
- ◦ A ⊆ X (that is, the FD is trivial) or
- ◦ X is a superkey of R or
- ◦ A is part of some candidate key (not just superkey!)

- Check if there are any transitive dependencies X->Y and Y->Z
- Decompose only if either LHS is a superkey OR RHS is a Prime Attribute.

#### BCNF - A relation schema R is in BCNF with respect to a set F of FDs if for all FDs in F + of
the form
α → β, where α ⊆ R and β ⊆ R at least one of the following holds:
- ◦ α → β is trivial (that is, β ⊆ α)
- ◦ α is a superkey for R

- Of all the Functinal dependencies that are applicable on the decomposed relations, check whether LHS is a super key in that table or not. If yes they are in BCNF else decompose further.

#### MVD -
If α → β, then α →→ β

#### 4NF - 
A relation schema R is in 4NF with respect to a set D of functional and multivalued
dependencies if for all multivalued dependencies in D + of the form α →→ β, where α ⊆
R and β ⊆ R, at least one of the following hold:
- ◦ α →→ β is trivial (that is, β ⊆ α or α ∪ β = R)
- ◦ α is a superkey for schema R

#### Further NFs
- ◦ Elementary Key Normal Form (EKNF)
- ◦ Essential Tuple Normal Form (ETNF)
- ◦ Join Dependencies And Fifth Normal Form (5 NF) [project-join normal form (PJNF)]
- ◦ Sixth Normal Form (6NF)
- ◦ Domain/Key Normal Form (DKNF)


