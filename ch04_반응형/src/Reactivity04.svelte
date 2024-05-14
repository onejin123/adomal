<script>
    //상태변수
    let count = 1;

    //반응성 코드 조건절
    $: if(count >= 10){
        alert('10개 이상 구매할 수 없습니다.');
        count = 9;
    }
    $: if(count <= 0){
        alert('최소 구매개수는 1개입니다.');
        count = 1;
    }

    //이벤트함수
    const onPlus = () => count++
    const onMinus = () => count--
</script>

<button on:click={onPlus}>+</button>
<input type="text" value={count} style="width: 25px;" />
<button on:click={onMinus}>-</button>
