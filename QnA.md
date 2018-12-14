# 질문을 올려주세요!!!

## Q1.프로세서 성능 분석 식에서 "(seconds/cycle)"이 1개 cycle이 실행하는데 걸리는 시간을 의미하는건가요?

>
> 네. "second/cycle"은 한 싸이클의 주기 시간을 의미합니다. 그리고 식에서 "cycle"은 1초당 나올 수 있는 클럭 주파수에 해당합니다.
>
> 예를 들어, 1GHz 마이크로프로세서의 경우, 초당 10^9 (10억)개의 cycle이 발생하는 것이고, 이때 한 cycle의 주기는 10^(-9) (1 nano second)이 됩니다.
>
> 식 "second/cycle"에서 좀더 의미를 잘 반영하려면, cycle 대신 clock frequency라고 쓰는 것이 더 좋을 수 있겠습니다.
>
> 따라서, 특정 마이크로프로세서에서 특정 SW의 수행 시간은 다음과 같이 기술될 수 있습니다.
>
> Execution_Time = (Total Number of Instructions) * (cycle / instruction) * (second / clock_frequency)
>
> 여기서 second를 1초로 해보면,
>
> Execution_Time = (Total Number of Instructions) * (cycle / instruction) * (1 / clock_frequency)
>
> (1 / clock_frequency) 는 한 클럭 사이클의 시간 즉 주기인거죠.
>

## Q2

```asm
        ;;17년 가을 기말고사 중
        addi	$sp, $zero, 8
        lw	$t0, -8($sp)
        lw	$t1, -8($sp)
        sub	$t2, $t0, $t1
        beq	$t2, $zero, LLL
        add	$t2, $s0, $s1
        sub	$t3, $s0, $s1
LLL:	  add	$t1, $t2, 8
        sub	$t3, $t2, $t1
        sw	$t1, -4($sp)
        sw	$t3, -8($sp)
```

5:5점)위 프로그램이 끝난 후 “메모리 4번지”에 저장되어 있는 값은 무엇인가 ?
이거에서 메모리 4번지에 저장되어 있는 값은 $t1이라 하셨는데 이해가 잘 되지 않아 추가 설명이 필요합니다.

> 답변>
>
> 마지막에서 두번째 명령어인
> sw	$t1, -4($sp)
>
> 이 4번지에 $t1을 저장하게 됩니다.
> $sp에 8이 들어가 있기 때문이죠.
