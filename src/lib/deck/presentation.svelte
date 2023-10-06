<script lang="ts">
	import Code from '$lib/deck/code.svelte'
	import Slide from '$lib/deck/slide.svelte'
	import Markdown from '$lib/deck/markdown.svelte'
	import Notes from '$lib/deck/notes.svelte'
</script>

<Slide>
	<h1>Slide 1</h1>
</Slide>

<Slide animate>
	<Code id="code" lines>
		{`
      function name(params:type) {
        
      }
    `}
	</Code>
</Slide>

<Slide animate>
	<Code id="code" lines>
		{`
      function name(params:type) {
        console.log("svelte")
      }
    `}
	</Code>
</Slide>

<Slide animate>
	<p class="uppercase">Transition</p>
	<div class="flex place-content-center gap-2">
		<div data-id="box-1" class="h-[100px] w-[100px] bg-gray-700"></div>
		<div data-id="box-2" class="h-[100px] w-[100px] bg-gray-700"></div>
		<div data-id="box-3" class="h-[100px] w-[100px] bg-gray-700"></div>
	</div>
</Slide>

<Slide animate>
	<p class="uppercase">Transition</p>
	<div class="flex place-content-center gap-2">
		<div data-id="box-1" class="h-[200px] w-[200px] bg-red-700"></div>
		<div data-id="box-2" class="h-[200px] w-[200px] bg-green-700"></div>
		<div data-id="box-3" class="h-[200px] w-[200px] bg-blue-700"></div>
	</div>
</Slide>

<Markdown>
	{`
			## Markdown
			Hello
	
	`}
</Markdown>

<Markdown name="example.md" external></Markdown>

<Slide>
	<h1>Slide</h1>
	<Notes>This is smaple notes</Notes>
</Slide>
