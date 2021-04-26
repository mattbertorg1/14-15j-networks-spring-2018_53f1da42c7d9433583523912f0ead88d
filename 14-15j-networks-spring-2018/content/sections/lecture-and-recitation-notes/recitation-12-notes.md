---
course_id: 14-15j-networks-spring-2018
layout: course_section
menu:
  leftnav:
    identifier: 2ec1c32b4e76eb2c1162a12d99c0d41e
    name: Recitation 12 Notes
    parent: 9f4e8596124d1608f9e6b335a917765a
    weight: 110
parent_title: Lecture and Recitation Notes
title: Recitation 12 Notes
type: course
uid: 2ec1c32b4e76eb2c1162a12d99c0d41e

---

Topics
------

*   Bargaining on Networks
*   Contagion Models
*   Mean-Field Approximation

Recall
------

*   Take-it-or-leave-it offer:
    *   One party makes an offer.  
        Then, the other party accepts or rejects it.  
        Game end.
    *   The proposer takes all the surplus. 
*   Rubinstein's bargaining:
    *   One party makes an offer.  
        The other party accepts or rejects.  
        If rejected, he makes a counter offer.  
        Continue until a party accepts.
    *   The first proposer takes _1/(1 + δ)_. The offeree takes _δ/(1 + δ)_.

Bargaining on Networks
----------------------

What if there are two sellers?

*   Take-it-or-leave-it offer:  
    *   If _S1_ offers _p_, _S2_ has incentive to offer _p — ε_.
    *   Even if sellers make (simultaneous) offers, they receive 0. The buyer receives 1.
*   Rubinstein's bargaining:
    *   If _S__1_ offers _1/(1 + δ)_, _S__2_ has incentive to offer _1/(1 + δ) — ε_.
    *   Again, the sellers receive 0, the buyer takes it all. 

Contagion Models
----------------

Recall games with externalities

*   _N_ = \[0, 1\]
*   _Si_ = {Adopt, Not Adopt}
*     
    ![Games with externalities equation.](/coursemedia/14-15j-networks-spring-2018/4a315788e2ae30aee7e776502c0e6ccc_MIT14_15JS18_rec12d.png)  
    Where _X_ is the share of adoption. 

This has externalities, but network structure doesn't matter. In reality, you may register for Instagram not only because it is popular, but also because your friends have it. 

Consider undirected graph (_V_, _E_), _N_(_i_) ⊂ _V_  
Where _V_ are vertices, _E_ are edges, and _N_ is the set of neighbors of vertex _i_ ∈ _V_.

*   _N_ = _V_
*   _Si_ = {Adopt, Not Adopt} = {1, 0}.
*     
    ![Undirected graph mathematical formula.](/coursemedia/14-15j-networks-spring-2018/ebe54f2e003bb4f7f555c8a6162e47ba_MIT14_15JS18_rec12a.png)

### _Example_

![Diagram of connected vertices](/coursemedia/14-15j-networks-spring-2018/730cf58198bc35247301325c83d4c238_MIT14_15JS18_rec12b.png)

*   Too complicated to solve (many-body problem).
*   Nor do we care about particular solution on particular networks. Often concerned with particular degree distribution, but not finer details.
*   Mean-field approximation to solve for stationary equation. 

To solve:

1.  Consider random graph with the degree distribution and fix some neighbor adoption probability _X_. 
2.  Obtain best response strategy given _X_ and compute adoption share _X̂_.
3.  Derive fixed point. 

### _Example_

Let _N_ = _V_ = \[0, 1\] and 

 ![Graph equation](/coursemedia/14-15j-networks-spring-2018/bb8b417c87219fb78a792637521a92c1_MIT14_15JS18_rec12c.png)

*   Agents are heterogeneous _ci_ ~ _F_(0, 1).
*   Degree distribution _d__i_ ~ _D_.

To solve:

1.  Fix some _X_. Pick agent _i_ randomly.
2.  _i_ with _c__i_ and _d__i_ would adopt if  
    ![Adoption equation.](/coursemedia/14-15j-networks-spring-2018/bdba4e6e80f64c4dca15c2562a751350_MIT14_15JS18_rec12e.png)
3.  Since _ci_ ~ _F_\[0, 1\], the probability that a random person with degree _d__i_ (but unknown _c__i_) adopts is _F_(_V_(_d__i_, _X_)). Since _d__i_ ~ _D_, we have the share of adoption 𝔼D\[_F_(_V_(_d__i_, _X_))\] . From here, we can compute the neighbor adoption share _X̂_.