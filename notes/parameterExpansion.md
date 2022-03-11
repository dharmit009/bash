# Parameter Expansion: 

It is the preferred way to set default values in **Bash**.

# What is parameter expansion?

This technique allows for a variable to be assigned a value if another
variable is either empty or is undefined.
 
**NOTATION:**

`${variableName:-default-value}`

The above line means if value for variable is null then set it the
given value. 

**Example:**

```bash
#!/usr/bin/env bash 

name="$1"
echo "${name:-'Please Provide a NAME as an argument'}"

if [[ -z "$1" ]];
then 
  echo "Now try running the script with parameter"
else [[ -n "$1" ]]
  echo "Now try running the script without any parameter"
fi 

```
