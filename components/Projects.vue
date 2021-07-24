<template>
	<div class='lg:w-1/2 mx-auto h-full flex flex-col divide-y-2 divide-gray-600 divide-opacity-25 px-10 mb-4'>
		<div v-for="(item, i) in projects" :key="i" class="flex w-full flex-col text-center lg:text-left" :class="{'lg:flex-row-reverse': i % 2 == 1, 'lg:flex-row': i % 2 == 0}">
			<img :src="item.img" class="mx-auto lg:mx-2 w-1/3 h-1/3 lg:w-1/5 lg:h-2/5 my-4 p-1 lg:p-5 my-auto">
			<div class="flex flex-col w-2/3 lg:w-4/5 my-4 mx-auto lg:mx-0">
				<p class="text-2xl font-medium">{{item.name}}</p>
				<p class="text-xl font-medium">{{item.time}}</p>
				<p class="text-md mb-2">{{item.desc}}</p>
				<div class="flex flex-row flex-wrap">
					<code v-for="(name, j) in item.tech" :key="j" class="bg-gray-100 text-xs p-0.5 mr-2 mb-2 rounded border">{{name}}</code>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	data: () => {
		return {
			projects: [
				{
					name: 'Plannet',
					time: '2020',
					img: 'plannet.png',
					desc: `At my high school's annual hackathon, hackBCA, I worked with a team to design an app that would allow users to 
						easily plan hangouts with their friends and track each other's availability. The project utilized Google's account API 
						and allowed for the creation of groups and event plans which the users could commit to.`,
					tech: ['html/css', 'javascript', 'jquery', 'node.js', 'google oauth', 'google maps api']
				},
				{
					name: 'UnionBlue',
					time: '2021',
					img: 'unionblue.png',
					desc: `For my senior capstone computer science project at BCA, I helped create a website for a friend's client that would 
					display PPE inventory for the Teamster's labor union and facilitate contact between the union and the PPE distributor through 
					a secure email form. The website also offered an admin view for creating, updating, and deleting items in stock.`,
					tech: ['pug html', 'tailwind css', 'sass', 'javascript', 'vue', 'express.js', 'vite']
				}
			]
		}
	}
}
</script>