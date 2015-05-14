# Semantic Analyzer for Cool

Made for Compilers course @ FCI-CU, 2015. Not meant to be used by the public. Assignment description is here http://www.acadox.com/class/16939#resources

Some notes to myself:
- Do NOT forget to check for double definition. i.e., if something has been defined twice.
- Do NOT forget to edit attr_class traversal to remove the condition, and find a way to not check for the inherited or coming-from-somewhere-else declarations.


Will write here last commit's changes:
- Fixed a bug in checking for redeclaration. I used to use lookup, although I should've used probe. Also, added it as well for the classes.
- Added method_class traverse implementation. Didn't add traversers for what it uses yet.
- In general, made expressions' types evaluate to No_type in case an error happened.
