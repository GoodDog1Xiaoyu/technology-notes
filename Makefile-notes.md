# 1. Official concepts:
The official introduction of rules is already good enough to understand the basic makefile:  
## 1.1 [The introduction of rules: It introduce the concept of target, prerequisites and recipe](https://www.gnu.org/software/make/manual/html_node/Rule-Introduction.html#Rule-Introduction)  
## 1.2. [There might exist some target names phony targets, which do not actually build any target and don't have prerequisites, only have recipes to run a series of commands](https://www.gnu.org/software/make/manual/html_node/Phony-Targets.html#Phony-Targets)

# 2. Some other related concepts:
## 2.1 The environment variables & make variables:  
Variables in make can come from the environment in which make is run. Every environment variable that make sees when it starts up is transformed into a make variable with the same name and value. However, an explicit assignment in the makefile, or with a command argument, overrides the environment.

# 3. Some tricks:
## 3.1 When write sed clause in make file, $ should be write as $$, and there might have more problems when sed includes #, ^, because make may expand it in some weird contents.