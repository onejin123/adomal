<script>
/* inline 이벤트 사용
- 이벤트를 제어할 경우 보통 함수를 만들어 이벤트와 연동하는 것이 보통입니다.
- 하지만 간단한 작업은 화살표 함수를 사용해서 마크업 영역에 인라인 형태로 사용할 수 있습니다. 
- Event02.svelte의 코드를 inkine 형태로 작성
*/
    //상태변수
    let m = {
        x: 0,
        y: 0
    }

    //
</script>

<div on:mousemove={e => m = {x : e.clientX, y : e.clientY}}>
    x좌표 : {m.x}<br />
    y좌표 : {m.y}
</div>

<style>
    div{
        width: 100%; height: 100%;
        background-color: pink;
    }
</style>