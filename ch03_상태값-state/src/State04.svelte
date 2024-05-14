<script>
    //상태변수선언
    let num = 0; //초기값 배정

    //기존 변수값에서 1씩 증가하는 함수
    const increaseNumber = () => num++
    
    //기존 변수값에서 1씩 감소하는 함수
    const decreaseNumber = () => num--
</script>

<button on:click={increaseNumber}>+</button>
<button on:click={decreaseNumber}>-</button>
<hr />
<h1>클릭횟수 : { num }</h1>