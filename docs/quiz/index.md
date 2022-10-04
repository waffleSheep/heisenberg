# Quiz
<script>
		function mark(element, num, correct) {
			if (correct) {
				element.style.color = 'green';
				document.getElementById('explanation'+num).style.display = 'block';
				document.getElementById('incorrect'+num).style.display = 'none';
			} else {
				element.style.color = 'red';
				document.getElementById('explanation'+num).style.display = 'none';
				document.getElementById('incorrect'+num).style.display = 'block';
			}
		}
	</script>
	


## Q1: Which one of the following phenomena suggest that light has particle-like properties?

<button class='md-button' onClick="mark(this, 1, false)">Polarisation of light</button> 
<br><br>
<button class='md-button' onClick="mark(this, 1, true)">Photoelectric effect</button> 
<br><br>
<button class='md-button' onClick="mark(this, 1, false)">The double-slit experiment</button> <br><br>
<button class='md-button' onClick="mark(this, 1, false)">The Davisson-Germer experiment</button> 
<br><br>

<section id='incorrect1' style="display:none;" markdown="block"> 
!!! failure "Incorrect!"
	Try again?
	
	![image](img/sad.jpg){ style=width:200px  }
</section>
<section id='explanation1' style="display:none;" markdown="block"> 
!!! success "Correct!"
	**Polarisation of light** and the **double-slit experiment** both showcase the *wave-like properties* of light. The **Davission-Germer experiment** shows the *particulate nature of electrons* rather than light. Hence, only the **photoelectric effect** showed that light was emitted in discrete packets.
	
	![image](img/happy.jpg){ style=width:200px }
</section>
<hr>



## Q2: Why?
### Give answers to three siginficant digit

<button class='md-button' onClick="mark(this, 2, false)">A</button> 
<br><br>
<button class='md-button' onClick="mark(this, 2, false)">B</button> 
<br><br>
<button class='md-button' onClick="mark(this, 2, true)">C</button> 
<br><br>
<button class='md-button' onClick="mark(this, 2, false)">D</button> 
<br><br>

<section id='incorrect2' style="display:none;" markdown="block"> 
!!! failure "Incorrect!"
	Try again?
	
	![image](img/sad.jpg){ style=width:200px  }
</section>
<section id='explanation2' style="display:none;" markdown="block"> 
!!! success "Correct!"
	Arbitrary something something
	
	![image](img/happy.jpg){ style=width:200px }
</section>
<hr>