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

**A. Polarisation of light** <br>
**B. Photoelectric effect** <br>
**C. The double-slit experiment** <br>
**D. The Davisson-Germer experiment**<br>

<button class='md-button' onClick="mark(this, 1, false)">A</button> 
<button class='md-button' onClick="mark(this, 1, true)">B</button> 
<button class='md-button' onClick="mark(this, 1, false)">C</button>
<button class='md-button' onClick="mark(this, 1, false)">D</button> 
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



## Q2: Which of the following statements about Heisenberg's Uncertainty Principle is FALSE?

 **A. It states that it is impossible to measure both position and momentum with perfect precision.** <br>
 **B. A similar uncertainty relation exists between any two canonically conjugate variables.**<br>
 **C. It arises because we must disturb a system in the process of measuring it (e.g. when we look at an object, a photon must have collided with it imparting momentum)**<br>
 **D. It is almost impossible to notice in daily life because $h$ is very small.**<br>
 
<button class='md-button' onClick="mark(this, 2, false)">A</button> 
<button class='md-button' onClick="mark(this, 2, false)">B</button> 
<button class='md-button' onClick="mark(this, 2, true)">C</button> 
<button class='md-button' onClick="mark(this, 2, false)">D</button> 
<br><br>

<section id='incorrect2' style="display:none;" markdown="block"> 
!!! failure "Incorrect!"
	Try again?
	
	![image](img/sad.jpg){ style=width:200px  }
</section>
<section id='explanation2' style="display:none;" markdown="block"> 
!!! success "Correct!"
	Heisenberg's uncertainty principle is an inherent property of all quantum systems. In certain interpretations, it is explained by the indeterminate nature of particles. The disturbance of a system in the process of conducting measurements is a separate phenomenon known as the **observer effect**. But even if we could perfectly measure a quantity without changing the system, the uncertainty principle would still hold!
	
	![image](img/happy.jpg){ style=width:200px }
</section>
<hr>

## Q3: Which of the following was the first form of the uncertainty principle, as suggested by Heisenberg in 1927?

 **A. $\Delta{x}\Delta{p_x} \sim h$** <br>
 **B. $\Delta{x}\Delta{p_x} = h$**<br>
 **C. $\Delta{x}\Delta{p_x} \geq\frac{h}{4\pi}$**<br>
 **D. $\Delta{x}\Delta{p_x} \sim \hbar$**<br>
 
<button class='md-button' onClick="mark(this, 3, true)">A</button> 
<button class='md-button' onClick="mark(this, 3, false)">B</button> 
<button class='md-button' onClick="mark(this, 3, false)">C</button> 
<button class='md-button' onClick="mark(this, 3, false)">D</button> 
<br><br>

<section id='incorrect3' style="display:none;" markdown="block"> 
!!! failure "Incorrect!"
	Try again?
	
	![image](img/sad.jpg){ style=width:200px  }
</section>
<section id='explanation3' style="display:none;" markdown="block"> 
!!! success "Correct!"
	The more popular form $\Delta{x}\Delta{p_x} \geq\frac{h}{4\pi}$ would only be proposed by Earle Hesse Kennard later that year.
	
	![image](img/happy.jpg){ style=width:200px }
</section>
<hr>


## Q4: Max Planck was first to...

 **A. Observe the photoelectric effect** <br>
 **B. Determine the equation explaining blackbody radiation** <br>
 **C. Propose that light existed in localised packets** <br>
 **D. Propose that all matter possessed wave-like properties** <br>
 
<button class='md-button' onClick="mark(this, 4, false)">A</button> 
<button class='md-button' onClick="mark(this, 4, true)">B</button> 
<button class='md-button' onClick="mark(this, 4, false)">C</button> 
<button class='md-button' onClick="mark(this, 4, false)">D</button> 
<br><br>

<section id='incorrect3' style="display:none;" markdown="block"> 
!!! failure "Incorrect!"
	Try again?
	
	![image](img/sad.jpg){ style=width:200px  }
</section>
<section id='explanation3' style="display:none;" markdown="block"> 
!!! success "Correct!"
	These milestones were done by Hertz, **Planck**, Einstein and De Broglie respectively.
	
	![image](img/happy.jpg){ style=width:200px }
</section>
<hr>

## Q5: Which of the following phenomena CANNOT be understood using the Heisenberg Uncertainty Principle?

 **A. Quantum tunneling** <br>
 **B. The non-existence of electrons in the nucleus** <br>
 **C. How scanning electron microscopes work** <br>
 **D. Wave-function collapse** <br>
 
<button class='md-button' onClick="mark(this, 5, false)">A</button> 
<button class='md-button' onClick="mark(this, 5, false)">B</button> 
<button class='md-button' onClick="mark(this, 5, false)">C</button> 
<button class='md-button' onClick="mark(this, 5, true)">D</button> 
<br><br>

<section id='incorrect3' style="display:none;" markdown="block"> 
!!! failure "Incorrect!"
	Try again?
	
	![image](img/sad.jpg){ style=width:200px  }
</section>
<section id='explanation3' style="display:none;" markdown="block"> 
!!! success "Correct!"
	Wave-function collapse is still not well-understood, and is explained differently across different interpretations of quantum mechanics. But Heisenberg's Uncertainty Principle and its mathematical basis stands true across all interpretations.
	
	![image](img/happy.jpg){ style=width:200px }
</section>
<hr>

## Q6: Heisenberg's microscope suffered from one major issue, it being...

 **A. It treats the electron as a classical particle, in direct contradiction to quantum physics** <br>
 **B. It assumes that Compton recoil exists** <br>
 **C. Heisenberg forgot to divide by $4\pi$** <br>
 **D. Heisenberg should have just held down the electron with tweezers** <br>
 
<button class='md-button' onClick="mark(this, 6, true)">A</button> 
<button class='md-button' onClick="mark(this, 6, false)">B</button> 
<button class='md-button' onClick="mark(this, 6, false)">C</button> 
<button class='md-button' onClick="mark(this, 6, false)">D</button> 
<br><br>

<section id='incorrect3' style="display:none;" markdown="block"> 
!!! failure "Incorrect!"
	Try again?
	
	![image](img/sad.jpg){ style=width:200px  }
</section>
<section id='explanation3' style="display:none;" markdown="block"> 
!!! success "Correct!"
	The proof of this result is left to the reader as an exercise.
	
	![image](img/happy.jpg){ style=width:200px }
</section>
<hr>