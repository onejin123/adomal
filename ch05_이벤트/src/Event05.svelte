<script>
    //이벤트함수
    const handleClick = () => {
        let move = confirm('유튜브로 이동하시겠습니까?');
        move && location.assign('https://youtube.com')
    }; 
</script>

<h1>
    <a on:click|preventDefault={handleClick}
    href = "https://youtube.com"
    >유튜브 바로가기</a>
</h1>