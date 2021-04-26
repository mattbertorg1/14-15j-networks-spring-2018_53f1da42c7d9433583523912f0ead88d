---
course_id: 14-15j-networks-spring-2018
layout: course_section
menu:
  leftnav:
    identifier: cc345d8d6c56e8b8d5cb038086ccf41b
    name: Recitation 9 Notes
    parent: 9f4e8596124d1608f9e6b335a917765a
    weight: 80
parent_title: Lecture and Recitation Notes
title: Recitation 9 Notes
type: course
uid: cc345d8d6c56e8b8d5cb038086ccf41b

---

Topics
------

*   Games with homogeneous externalities
*   Games with local network effects

Recall
------

Congestion games had simple sets of payoffs but complicated network structure. There are games that have complicated payoffs with simple network structure. 

Homogeneous Externalities
-------------------------

In classical economics, the demand curve is assumed decreasing and the supply curve increasing. The existence of network effects may create a weird shape of the demand curve. 

*   _N_ = \[0, 1\] continuum of players
*   _S__i_ \= {buy, not buy}
*   _u__i_(_S__i_, _S__\-i_) = _u__i_(_S__i_, _x_) =  
    _vix_ — _p_  if _S__i_ = buy  
    0           if _S__i_\= not buy
*   _v__i_ ~ F(\[0, 1\])
*   _p_ > 0
*   Where _x_ is how many buy, _v__i_ is its value, and _p_ is price.

### _Example: Office suites, SNS, etc._ 

![Diagram of network effects problem.](/coursemedia/14-15j-networks-spring-2018/735c3dc469f426c4a7c455839ab79bf3_MIT14_15JS18_rec9e.png)

*   _x_ = 1 — F(_v̅_) where _v̅_ is the lowest value of agents who buy.

Claim: If agent with _v__i_ = _v̅_ is better off buying, then any agent with _v__j_ > _v̅_ is also better off buying. 

Corollary: We may assume without loss of generality that _x_ (those who buy) have the highest values in equilibrium/socially optimal outcome. 

1.  Socially optimal outcome
    1.  Social welfare = _v̅_∫1\[_v_(1 — F(_v̅_)) — _p_\] dF(_v_)
    2.  Maximizing this with respect to _v̅_ yields the social best.
2.  Nash equilibrum
    1.  Pooling equilibrum:  
        If no one has the good (_x_ = 0) then no one has incentive to buy ( _v__i_ \* 0 — _p_ < 0). Therefore, _x__\*_ = 0 is an equilibrium. 
    2.  Separating equilibrium:  
        If someone buys (_x_ > 0), then there exists the lowest type _v̅_ who buys. His incentive must balance _v̅x_ — _p_ = 0.

Note that everyone's strategy is summarized by _x_. So consider the aggregate best response function BR(_x_) = _x̂_. With _v̅x_ — _p_ = 0 and _x_ = 1 — F(_v̅_), we find:

*   BR(_x_) = 1 — F(_p_/_x_).
*   Its fixed point _x__\*_ is an equilibrium. 

Local Network Effects
---------------------

Some games have both complicated payoff structure and complicated network structure.

 ![Diagram of substitutes and not substitutes for payoff structures.](/coursemedia/14-15j-networks-spring-2018/09c2914fedc070a5d7f46caf72833219_MIT14_15JS18_rec9d-2.png)

*   _N_ = {1, 2, 3}.
*   _S__i_ = ℝ\+ \= \[0, ∞).
*   _u__i_(_x__i_, _x__\-i_, δ, _G_) =   
    ![Local network effect equation.](/editor/coursemedia/14-15j-networks-spring-2018/8d7d11358ca647c16c660860dac6514f_MIT14_15JS18_rec9a.png)

_i_'s best response satisfies

![Best response equation.](/editor/coursemedia/14-15j-networks-spring-2018/1c9f3f1da0a7fc0487d444b1d6f7d4e2_MIT14_15JS18_rec9b.png)

*   ![Expanded best response equation. ](/coursemedia/14-15j-networks-spring-2018/2719373e98a6f5923bdf233060d0a0fb_MIT14_15JS18_rec9c.png)
*   BR(_x_) = max { 𝟘, 𝟙 — δ_G_𝕏}