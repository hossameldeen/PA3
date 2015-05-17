# Semantic Analyzer for Cool

Made for Compilers course @ FCI-CU, 2015. Not meant to be used by the public. Assignment description is here http://www.acadox.com/class/16939#resources

Some notes to myself:
- Do NOT forget to check for double definition. i.e., if something has been defined twice.
- Do NOT forget to edit attr_class traversal to remove the condition, and find a way to not check for the inherited or coming-from-somewhere-else declarations.
- Do NOT forget: In object_class::traverse(), you need to check whether the ID is defined through attribute, formal, let, or case.
- Do NOT forget: In some if-conditions you should've put `{}` but you didn't.


## What to do next?
Look at the table below and implement the unimplemented.
Probably, you'll need to implement:
- traverse for most nodes (NOT all). Sometimes the traverse does nothing. But usually, it sets the type of an expression.
- get_type() for expression nodes.

Ummm .. will write the state of each thing here isA. But now it'll be empty:
- program: Done.
- class: Done.
- feature as method: Done.
- feature as attribute: Done.
- formal: Done.
- assign_expr: Done.
- static_dispatch: Done. I modify a bit
- dispatch:Done
- cond_expr: Done.
- loop_expr: Done.
- block_expr: Done.
- let_expr: Done.
- branch_expr:
- new_expr: Done.
- isvoid_expr: Done.
- plus_expr: Done.
- sub_expr: Done.
- mul_expr: Done.
- divide_expr: Done.
- comp_expr: Done
- less than_expr: Done.
- le_expr: Done.
- eq_expr: Done.
- not_expr: Done.
- parenthesis expr: Probably, won't need to do anything.
- object_expr: Done as idea, but not as code.
- int_const: Done.
- string_const: Done.
- boolean_const: Done.
- self things
-------------------------------
modifications in expression set type and check if type of an instance exist

testing:
class:
 - one class run correctly
 - two class run correctly
 - more class run
feature:
 - declare attributes run correctly
 - declare method with any exist return type run  correctly

 dispatch:
  - fixed 
  - dispatch with parameter work correctly

------------------
Will make an analogy with the above:
- program: Done.
- class: Done. one or more Done.
- feature as method: Done.
- feature as attribute: Done.
- formal: Done.
- assign_expr: Done.
- static_dispatch: Done.
- dispatch: Done.
- cond_expr: Done.
- loop_expr: .
- block_expr: Done.
- let_expr: .
- branch_expr:
- new_expr: .
- isvoid_expr: .
- plus_expr: .
- sub_expr: .
- mul_expr: .
- divide_expr: .
- comp_expr: 
- less than_expr: .
- le_expr: .
- eq_expr: .
- not_expr: .
- parenthesis expr: Probably, won't need to do anything.
- object_expr:  as idea, but not as code.
- int_const: .
- string_const: .
- boolean_const: .
- self things
-------------------

-------------------------------
May write here last commits changes:
- Testing mentioned above.
- Handled SELF_TYPE.
- Fixed a bug in eq, leq, lt.
