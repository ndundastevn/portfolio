<template>
	<section class="">
		<h1>Hello world</h1>
		<p>
			Lorem, ipsum dolor sit amet consectetur adipisicing elit. dddddddddddddddddddddddddddddddddddddddddd
		</p>
	</section>
	<section class="">
		<div class="boxs">
			<div class="box hidden">

			</div>
			<div class="box hidden">

			</div>
			<div class="box hidden">

			</div>
			<div class="box hidden">

			</div>

		</div>
	</section>
	<section class="">
		<h1>Hello world</h1>
		<p>
			Lorem, ipsum dolor sit amet consectetur adipisicing elit. dddddddddddddddddddddddddddddddddddddddddd
		</p>
	</section>
	<section class="hidden">
		<h1>Hello world</h1>
		<p>
			Lorem, ipsum dolor sit amet consectetur adipisicing elit. dddddddddddddddddddddddddddddddddddddddddd
		</p>
	</section>

 </template>
 <script>
	const observer = new IntersectionObserver(entries => {
        entries.forEach(entry => {
          console.log(entry)
          if (entry.isIntersecting) {
            entry.target.classList.add('show');
          } else {
            entry.target.classList.remove('show');
          }
        })
      })

      const hiddenElements = document.querySelectorAll('.hidden')
      hiddenElements.forEach(el => observer.observe(el))
 </script>
 <style>


	section{
    background-color: white;
		color: black;
		display: grid;
		place-items: center;
		align-content: center;
		min-height: 100vh;
	}

	.hidden{
		opacity: 0;
		filter: blur(5px);
		transform: translateX(-100%);
		transition: all 2s;
	}

	.show {
		opacity: 1;
		filter: blur(0);
		transform: translateX(0);
	}

	@media(prefers-reduced-motion){
		.hidden{
			transition: none;
		}
	}
	.boxs{
		display: flex;
		gap: 6px;
	}

	.box{
		height: 150px;
		width: 150px;
		border-radius: 24px;
		background-color: white;
		display: flex;
	}

	.box:nth-child(2){
		transition-delay: 200ms;
	}
	.box:nth-child(3){
		transition-delay: 400ms;
	}
	.box:nth-child(4){
		transition-delay: 600ms;
	}

 </style>
