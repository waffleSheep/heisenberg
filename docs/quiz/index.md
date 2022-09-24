# Quiz hamburger
<script>
		function mark(element, num, correct) {
			if (correct) {
				element.style.color = 'green';
				document.getElementById('id'+num).innerText = "nice";
				document.getElementById('image'+num).src = "img/happy.jpg"
			} else {
				element.style.color = 'red';
				document.getElementById('id'+num).innerText = "oh no";
				document.getElementById('image'+num).src = "img/sad.jpg"
			}
		}
	</script>
	
filer ex

# Q1: What was xxxxxxxxxxx?
### Hint: (help me)

<div>
	<br><br>
	<button class='md-button' onClick="mark(this, 1, true)">SHFJHFHFLKSDFHKJSDFHdkjsfhdsjkfhsdjfhskahdjkghasdkjhslkjadhajfhalkjfhwakjehf</button> <br><br>
	<button class='md-button' onClick="mark(this, 1, false)">B</button> <br><br>
	<button class='md-button' onClick="mark(this, 1, false)">C</button> <br><br>
	<button class='md-button' onClick="mark(this, 1, false)">D</button> <br><br>
	<p id='id1'>yeah its going</p>
	<img id='image1' src="">
	<hr>
</div>


# Q2: Why?
### Give answers to three siginficant digit

<div>
	<br><br>
	<button class='md-button' onClick="mark(this, 2, false)">A</button> <br><br>
	<button class='md-button' onClick="mark(this, 2, false)">B</button> <br><br>
	<button class='md-button' onClick="mark(this, 2, true)">C</button> <br><br>
	<button class='md-button' onClick="mark(this, 2, false)">D</button> <br><br>
	<p id='id2'></p>
	<img id='image2' src="">
</div>