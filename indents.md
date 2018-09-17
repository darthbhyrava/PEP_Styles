# 1. Consistency
***
"A foolish inconsistency is the hobgoblin of little minds."
While consistency is desirable across functions, modules, packages, projects,
teams and organizations, you shouldn't stick to it for the sake of it:
	- don't break backwards compatibility 
	- don't make code less readable
	- don't change predated code
	- don't compromise on code compatibility

# 2. Code Lay-Out
***
## 2.1 Code Indentation
- Aligned with opening delimiter:
```
foo = long_function_name(var_one, var_two,
						 var_three, var_four)
```
- More indentation to distinguish
```
def long_function_name(
		var_one, var_two, var_three,
		var_four):
	print(var_one)
```
- Hanging indents should add a level
```
foo = long_function_name(
	var_one, var_two,
	var_three, var_four)
```
