
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
```
# $s0 = pow, $s1 = x
# int pow = 1;
	addi	$s0, $0, 1
# int x   = 0;
	add	$s1, $0, $0
	addi	$t0, $0, 128
돌아라:
#  pow = pow * 2;
	sll	$s0, $s0, 1
#  x = x + 1;
	addi	$s1, $s1, 1
	bne	$s0, $t0, 돌아라

```

```
// add the numbers from 0 to 9
int sum = 0;
int i;

for (i=0; i != 10; i = i+1) {
  sum = sum + i;
}

=>>

# $s0 = i, $s1 = sum
	addi	$s1, $0, 0
	addi	$s0, $0, 0
	addi	$t0, $0, 10

올려줘:	beq	$s0, $t0, 나가
	# for loop body : sum = sum + i
	add	$s1, $s1, $s0
	# i = i + 1
	addi	$s0, $s0, 1
	j	올려줘
나가:

```
