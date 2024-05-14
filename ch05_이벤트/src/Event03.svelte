<script>
/*
매개변수가 있는 함수를 마크업 문법에 이벤트 핸들러로 지정할 때
람다로 감싸줘야 한다. 그렇지 않으면 요소가 로드될 때 이벤트가 실행되게 된다.
*/
    //이벤트함수
    const handleClick = text => alert(`${text}클릭`);
</script>

<button on:click={() => handleClick('1번')}>버튼</button>
<button on:click={() => handleClick('2번')}>버튼</button>
