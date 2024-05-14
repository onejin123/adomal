<script>
    //상태변수
    let m = {
        x: 0,
        y: 0
    }

    //이벤트함수
    const handleMouseMove = e => {
        m.x = e.clientX;
        m.y = e.clientY;
    }

    /* DOM 이벤트 사용
    function handleMousemove(event){
		m.x = event.clientX;
		m.y = event.clientY;
	}
    */
</script>

<div on:mousemove={handleMouseMove}>
    x좌표 : {m.x}<br />
    y좌표 : {m.y}
</div>

<style>
    div{
        width: 100%; height: 100%;
        background-color: pink;
    }
</style>