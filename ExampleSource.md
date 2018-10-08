
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

```

 * SLT (Set Less Than : 작은면 설정해! 
   [slt  R3, R1, R2]
	
	if( R1 < R2 ) R3 <- 1
	else R3 <- 0

   // C 언어의 Ternary operator (삼항 연산자)
   R3 = (R1 < R2) 1 : 0;
================================
# add the powers of 2 from 1 
# to 100
# $s0 = i, $s1 = sum
# int sum = 0;
	addi	$s1, $0, 0
# int i=1
	addi 	$s0, $0, 1
	addi	$t0, $0, 101
	addi	$t3, $0, 1
위로:
	# i < 101 돌아야!
	slt	$t1, $s0, $t0    # $t1 ==1 gogo 아니면 나가야지!
	bne	$t1, $t3, 나가
	# sum = sum + i;
	add	$s1, $s1, $s0
	# i = i*2
	sll	$s0, $s0, 1
	j	위로
나가:






```
