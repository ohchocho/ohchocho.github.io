<<<<<<< HEAD
# ckick Event

**[js] 자바스크립트 onclick · addEventListener 비교 사용법**

---



# 1. onclick 이벤트

onclick은 모든 브라우저와 버전에서 호환이 됩니다.



### 1-1. HTML 코드에서 inline 방식

자바스크립트를 지원하는 모든 브라우저에서 HTML코드에 바로 이벤트 리스너를 넣는다.

●단점 : 가독성이 안좋아지며, 유지보수가 힘들다.

```jsx
<input type="button" id="target3" onclick="alert('Hello World')" value="alertBtn_this_inline">
```



### 1-2. 자바스크립트에 onclick 이벤트 작성

●단점 : 단 하나의 이벤트 리스너만을 사용할 수 있다.

```jsx
<input type="button" id="target4" value="프로퍼티 방식">
<script>
	onst t = document.getElementById('target4');
	t.onclick = function() {
	    alert("프로퍼티 방식")
	}
</script>
```





# 2. addEventListener 메서드

● 가장 추천하는 모던한 방식이다.

addEventListener는 여러 개의 이벤트 리스너를 추가(사용) 할 수 있습니다.

`addEventListener()` 는 거의 모든 브라우저에서 지원하는 이벤트 리스너 작성(등록)을 위한 메서드이다.

`addEventListener()` 메서드에는 'on'이 붙지 않는다.

●단점 : Internet Explorer 6,7,8 에서는 호환되지 않으므로 대신에 이와 유사한 동작을 하는 attachEvent() 메서드와 detachEvent() 메서드를 사용해야 합니다.

```jsx
<input type="button" id="target4" value="프로퍼티 방식">
<script>
const add = document.getElementById('target4');
    add.addEventListener('click', function() {
        alert("addEventListener")
    });
</script>
```



### 따라서,

onclick에는 하나의 콜백 함수(리스너)만 지정할 수 있다.  

만약 onclick 이벤트 핸들러를 두 번 이상 사용한다면, 기존 이벤트 핸들러를 덮어쓰기 때문에 가장 아래에 추가한 핸들러만 작동합니다.



### 그러므로,

위의 구형 브라우저 호환성의 문제가 있다면 onclick을 사용하지만, 

그 외에는 개발자가 추천하는 모던한 방식의 **addEventListener 사용을 추천**합니다.
=======
# ckick Event

**[js] 자바스크립트 onclick · addEventListener 비교 사용법**

---



# 1. onclick 이벤트

onclick은 모든 브라우저와 버전에서 호환이 됩니다.



### 1-1. HTML 코드에서 inline 방식

자바스크립트를 지원하는 모든 브라우저에서 HTML코드에 바로 이벤트 리스너를 넣는다.

●단점 : 가독성이 안좋아지며, 유지보수가 힘들다.

```jsx
<input type="button" id="target3" onclick="alert('Hello World')" value="alertBtn_this_inline">
```



### 1-2. 자바스크립트에 onclick 이벤트 작성

●단점 : 단 하나의 이벤트 리스너만을 사용할 수 있다.

```jsx
<input type="button" id="target4" value="프로퍼티 방식">
<script>
	onst t = document.getElementById('target4');
	t.onclick = function() {
	    alert("프로퍼티 방식")
	}
</script>
```





# 2. addEventListener 메서드

● 가장 추천하는 모던한 방식이다.

addEventListener는 여러 개의 이벤트 리스너를 추가(사용) 할 수 있습니다.

`addEventListener()` 는 거의 모든 브라우저에서 지원하는 이벤트 리스너 작성(등록)을 위한 메서드이다.

`addEventListener()` 메서드에는 'on'이 붙지 않는다.

●단점 : Internet Explorer 6,7,8 에서는 호환되지 않으므로 대신에 이와 유사한 동작을 하는 attachEvent() 메서드와 detachEvent() 메서드를 사용해야 합니다.

```jsx
<input type="button" id="target4" value="프로퍼티 방식">
<script>
const add = document.getElementById('target4');
    add.addEventListener('click', function() {
        alert("addEventListener")
    });
</script>
```



### 따라서,

onclick에는 하나의 콜백 함수(리스너)만 지정할 수 있다.  

만약 onclick 이벤트 핸들러를 두 번 이상 사용한다면, 기존 이벤트 핸들러를 덮어쓰기 때문에 가장 아래에 추가한 핸들러만 작동합니다.



### 그러므로,

위의 구형 브라우저 호환성의 문제가 있다면 onclick을 사용하지만, 

그 외에는 개발자가 추천하는 모던한 방식의 **addEventListener 사용을 추천**합니다.
>>>>>>> 6bb49466954e286c11e6060721b12670cd409ae0
