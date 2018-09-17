# 1. Consistency
"A foolish inconsistency is the hobgoblin of little minds." 
While consistency is desirable across functions, modules, packages, projects,
teams and organizations, you shouldn't stick to it for the sake of it: 
    - don't break backwards compatibility 
	- don't make code less readable 
	- don't change predated code 
	- don't compromise on code compatibility 

# 2. Code Lay-Out
## 2.1 Code Indentation
Dealing with indentation in more general cases: 
- Aligned with opening delimiter
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
- Hanging indents should add a level (__IT'S-__)
``` 
foo = long_function_name(
	var_one, var_two,
	var_three, var_four)
```
- Hanging indents have spaces optional for the 'hanging' part
```
foo = long_function_name(
  var_one, var_two,
  var_three, var_four)
```
__DO NOT:__
- Put arguments on first line forbidden when not using vertical alignment
```
foo = long_function_name(var_one, var_two,
	var_three, var_four)
```
- Forget to use extra indentation when not evident
```
def long_function_name(
	var_one, var_two, var_three,
	var_four):
	print(var_one)
```
In _if_ statements, the `if (` is 4 spaces long, hence visual confusion with 
the next line. Multiple ways to deal with this are: 
- No extra charge
```
if (this is one line
    and this another)
    do_nothing()
```
- Add a comment, which will provide some distinction in editors supporting 
syntax highlighting.
```
if (this_is_one_thing and
    that_is_another_thing):
    # Since both conditions are true, we can proceed.
    do_something()
```
- Add some extra indentation on the conditional continuation line.
if (this_is_one_thing
        and that_is_another_thing):
    do_something()
