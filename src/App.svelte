<script>
	import AppBar from "./components/AppBar.svelte";
	import RaisedButton from "./components/RaisedButton.svelte";
	import OutlineButton from "./components/OutlineButton.svelte";
	import Card from "./components/Card.svelte";
</script>

<AppBar title={{ label: "Hello World", onClick: () => console.log("Hello World") }} navLinks={[{label: "Link1", route: "/"}, {label: "Link2", route: "/"}, {label: "Link3", route: "/"}]}/>

<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} />

<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} darkMode={"true"} />

<OutlineButton label={"Hello World"} onClick={() => console.log("Button Clicked")} />

<Card>
	<h1 class="text-3xl">Hello World</h1>
	
	<p class="text-md text-left">Sunt dolor est elit proident laboris qui laboris. Enim in ullamco ex laboris veniam elit laborum eiusmod veniam veniam ex. Consectetur cupidatat qui laborum laborum cillum dolore minim. Tempor laborum aliquip qui consequat. Et ex nulla occaecat nulla mollit reprehenderit voluptate labore est dolore.</p>
	
	<br>

	<p class="text-md text-left">Duis nisi non occaecat esse magna voluptate sunt eiusmod est veniam excepteur non ullamco eiusmod. Tempor enim consectetur sit sint dolor ad cupidatat minim. Non ad reprehenderit aliquip aute esse exercitation aute sint reprehenderit ut do culpa eiusmod.</p>

	<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} darkMode={"true"} />

	<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} />
</Card>