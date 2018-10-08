
=========================
```
# $s0 = f, $s1 = g, $s2 = h
# $s3 = i, $s4 = j


	bne $s3, $s4, ELSE
THEN:	add $s0, $s1, $s2
	j      IF_END
ELSE:
	sub $s0, $s0, $s3
IF_END:


if (i == j)
  f = g + h;
else
  f = f – i;
```
=========================
