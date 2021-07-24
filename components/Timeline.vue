<template>
	<div class="container mx-auto w-full h-full mb-4">
		<div class="relative wrap overflow-hidden p-10 h-full">
			<div class="absolute bg-gray-800 bg-opacity-20 h-full w-0.5" style="left: 49.9%"></div>

			<div v-for="(item, i) in items" :key="i" class="mb-8 flex justify-between items-center w-full" :class="{'flex-row-reverse': i % 2 == 1}">
				<div class="order-1 w-5/12"></div>
				<div class="z-20 flex items-center order-1 bg-gray-800 shadow-xl w-8 h-8 rounded-full"></div>
				<div class="order-1 rounded-lg shadow-xl w-5/12 px-6 py-4 text-gray-800" :class="{'bg-blue-400': i % 2 == 0, 'bg-red-400': i % 2 == 1}">
					<p class="mb-0 font-bold text-xl" :class="{'text-white': i % 2 == 1}">{{item.title}}</p>
					<p class="mb-1 font-bold text-xl" :class="{'text-white': i % 2 == 1}">{{item.place}}</p>
					<p class="mb-3 text-lg" :class="{'text-white': i % 2 == 1}">{{item.time}}</p>
					<p class="mb-2 text-sm leading-snug tracking-wide text-opacity-100" :class="{'text-white': i % 2 == 1}">{{item.desc}}</p>
					<div class="flex flex-row flex-wrap">
						<code v-for="(name, j) in item.tech" :key="j" class="bg-gray-100 text-xs p-0.5 mr-2 mb-2 rounded border">{{name}}</code>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	data: () => {
		return {
			items: [
				{
					'title': 'Student',
					'place': 'Bergen County Academies (BCA)',
					'time': '2017-2021',
					'desc': `As a student in the Academy of Technology and Computer Science, I studied discrete mathematics, linear algebra, 
						algorithms, data structures, field and set theory, object-oriented programming, functional programming, 
						web development, and more. 
						I gained valuable project experience working on BCA's student dashboard backend, independent projects 
						under the mentorship of my teachers, and a culminating senior capstone project.`,
					'tech': ['python', 'java', 'object oriented programming', 'sql', 'html/css', 'php', 'flask', 'c', 'data structures', 'algorithms', 'linux', 'functional programming', 'racket', 'networking']
				},
				{
					'title': 'Teacher',
					'place': 'Hasbrouck Heights Public Library',
					'time': '2019-2020',
					'desc': `Working with the library director, I organized two free, 10-week programming courses available to students 
						attending Hasbrouck Heights Middle School. The class taught programming fundamentals as part of a curriculum that I 
						designed.`,
					'tech': ['python', 'teaching']
				},
				{
					'title': 'Software Engineer Intern',
					'place': 'Bloomberg L.P.',
					'time': '2020-2021',
					'desc': `As a part of the Bloomberg Law (BLAW) Release Engineering Team, I worked on a dashboard for BLAW's permissions 
						database. This dashboard enables team leads to get insights on the permissions that their developers have created, along 
						with how long they will last if they are temporary. The dashboard also has a view of all the permissions in the database and 
						a diff generator that shows the differences in permissions between the alpha, beta, and production environments. 
						Additionally, it offers tools for directly creating, updating, deleting, and moving permissions between the three environments 
						through a RESTful API.`,
					'tech': ['java', 'maven', 'spring framework', 'postgresql', 'aspect oriented programming', 'rest api', 'ruby on rails', 'graphql', 'javascript', 'vue']
				},
				{
					'title': 'Student',
					'place': 'University of Maryland, College Park',
					'time': '2021-2025',
					'desc': `I will be majoring in computer science at the College of Computer, Mathematical, and Natural Sciences.`,
					'tech': []
				},
			]
		}
	}
}
</script>