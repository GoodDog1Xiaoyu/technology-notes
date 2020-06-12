# Some little knowledges

1. Sometimes we gurantee that some variable must be there, so we avoid NULL check and just let it crash which can be more easily to find the problems.

2. Nested function in C:
Nested function is allowed in some C compilers, nested function have its own stack call, but can access to the fuctions's local variables that it is nested. 

**This is a good point to do some research on the compilers accross different platform.**

3. Different shells may have some different behavior for some linux commands.

4. #ifdef conditional definition can be used when add some new feature in the newer version. When we add test case, if some test cases only work for then newer version. Since we might not know what the binary we used to test (new or old, we can conditional compile them, so that if use the old binary, it will not lead to compile crash).