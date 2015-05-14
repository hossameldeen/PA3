# Semantic Analyzer for Cool

Made for Compilers course @ FCI-CU, 2015. Not meant to be used by the public. Assignment description is here http://www.acadox.com/class/16939#resources

Some notes to myself:
- Do NOT forget to check for double definition. i.e., if something has been defined twice.
- Do NOT forget to edit attr_class traversal to remove the condition, and find a way to not check for the inherited or coming-from-somewhere-else declarations.
- Do NOT forget: In object_class::traverse(), you need to check whether the ID is defined through attribute, formal, let, or case.


Ummm .. will write the state of each thing here isA. But now it'll be empty:
- program:
- class:
- feature as method:
- feature as attribute:
- formal:
- assign_expr:
- static_dispatch:
- dispatch:
- cond_expr:
- loop_expr:
- block_expr:
- let_expr:
- case_expr:
- new_expr:
- isvoid_expr:
- plus_expr:
- sub_expr:
- mul_expr:
- divide_expr:
- neg_expr:
- less than_expr:
- le_expr:
- eq_expr:
- not_expr:
- parenthesis expr: Probably, won't need to do anything.
- object_expr: Done as idea, but not as code.
- int_const: Done.
- string_const: Done.
- boolean_const: Done.
- self things