<script>
    //상태변수선언
    let artist = {
		name: '진',
		age: 31,
		height: 179,
		group: '방탄소년단',
		img: 'https://search.pstatic.net/sunny/?src=https%3A%2F%2Fw.namu.la%2Fs%2F8152fad7a07738b7d11b8fe1b44b3cd0db34d5fa5c35abee4deae2fd163a4218f003e753532e1edd20a4db12e88382c0f3342d054cba5a0d38ba8bd9be593138ae4b6404caf7373e92540f2688467b825caa89de860dccc282395d440f6f72db&type=fff264_180'
	}

    //비구조화할당
    let {name, age, height, group, img} = artist;
</script>

<h1><img src={img} alt="사진" /></h1>
<h1>이름 : {name}</h1>
<h1>나이 : {age}</h1>
<h1>키 : {height}</h1>
<h1>소속그룹 : {group}</h1>