<script> // 삼항연산자 예제
    //상태변수
    let count = 0;

    //이벤트함수
    const handleClick = () => count++;
</script>

<button on:click={handleClick}>
    클릭 수 : {count}
    {count <= 1 ? 'time' : 'times'}
</button>