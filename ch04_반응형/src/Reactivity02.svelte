<script>
    //상태변수
    let count = 0;

    //반응성 변수선언
    $: doubled = count * 2;
    $: square = count * count;

    //이벤트함수
    const handleClick = () => count++;
</script>

<button on:click={handleClick}>클릭 수 : {count}</button>
<h3>두배구하기</h3>
<p>{count} x 2 = {doubled}</p>
<h3>제곱구하기</h3>
<p>{count} x {count} = {square}</p>
