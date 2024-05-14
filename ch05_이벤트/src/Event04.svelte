<script>
/* Event Modifiers(이벤트 수식어)
- 이벤트명 뒤에 [ | ](파이프문자)를 통해 수식어를 붙일 수 있습니다. 
수식어	         설명
preventDefault	'e.preventDefault()' 를 호출. 이벤트가 발생한 태그의 기본 이벤트를 막음.
stopPropagation	'e.stopPropagation()' 을 호출. 발생한 이벤트가 겹쳐진 상위 요소로 전달되지 않게 막음.
passive	        터치 혹은 휠 이벤트로 발생하는 스크롤 성능을 향상시킴.
capture	        버블링 단계가 아닌 캡처 단계에서 이벤트 핸들러를 실행함.
once	        이벤트 핸들러를 단 한번만 실행하도록 함.
self	        'e.target'과 이벤트 핸들러를 정의한 요소가 같은 때 이벤트 핸들러를 실행하도록 함.
*/
    //이벤트함수
    const handleClick = text => alert(`${text}클릭`);
</script>

<button on:click|once={() => handleClick('1번')}>버튼</button>
<button on:click|once={() => handleClick('2번')}>버튼</button>
