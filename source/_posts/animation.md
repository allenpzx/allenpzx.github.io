---
title: JavaScript origin animation
date: {{ date }}
tags:
- JavaScript
- Animation

---

## JavaScript Origin animation



#### list animation

```js
	Array.from(lists).map((item, key)=>{
		setTimeout(()=>{
			item.style.transform = `translate(${}, ${})`;
		}, key * 100)
	})
```
<!-- more --> 


#### shuffle animation

```js
	let origin_arr = [];
	let shuffle_arr = _shuffle(origin_arr);

	shuffle_arr.map((item, key)=>{
		item.style.transform = `translate(${origin_arr[key].offsetLeft}, ${origin_arr[key].offsetLeft})`;
	})
```



#### gressive animation

```js
	window.requestAnimationFrame( animation_1 )

	animation_1 = () => {
		let item = document.getElementById(‘id’);
		if(item.offsetLeft > some value){
			item.style.left = some value
			return 
		}
		speed = parseFloat((target - current)/10);
		item.style.left += speed;
	}
```

