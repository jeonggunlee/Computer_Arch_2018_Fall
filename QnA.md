# 질문을 올려주세요!!!

## 프로세서 성능 분석 식에서 "(seconds/cycle)"이 1개 cycle이 실행하는데 걸리는 시간을 의미하는건가요?

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
