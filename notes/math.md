# Math in Bash 

**The best practice would be to use something like `bc`** for calculations
as the standard bash *does not support floating point operations* which 
is not the best. Though you can perform some arithmetic operations if you
like ... 

**Example:**

```bash 
#!/bin/bash

n1="$1"
n2="$2"
out=$((n1+n2))
echo "$out"

```

#!/bin/bash
$1=100
$2=200
n1="$1"
n2="$2"
out=$((n1+n2))
echo "$out"

