<script>
	import AppBar from "./components/AppBar.svelte";
	import Link from "./components/Link.svelte";
	import RaisedButton from "./components/RaisedButton.svelte";
	import OutlineButton from "./components/OutlineButton.svelte";
	import Card from "./components/Card.svelte";
	import TextField from "./components/TextField.svelte";
	import Form from "./components/Form.svelte";
	import Code from "./components/Code.svelte";
	import Accordion from "./components/Accordion.svelte";

	const codes = [
		"<h1>Hello World</h1>",
		"<p>Thanks for using SvelteDash</p>"
	];
</script>

<AppBar title={{ label: "Hello World", onClick: () => console.log("Hello World") }} navLinks={[{label: "Link1", route: "/"}, {label: "Link2", route: "/"}, {label: "Link3", route: "/"}]}/>

<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} />

<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} darkMode={"true"} />

<OutlineButton label={"Hello World"} onClick={() => console.log("Button Clicked")} />

<Link link={{ label: "This is a link", route: "/" }} />

<TextField label={"Hello World"} onChange={(newValue) => console.log(newValue)} />

<Card>
	<h1 class="text-3xl text-center">Hello World</h1>
	<p class="text-md text-left">Sunt dolor est elit proident laboris qui laboris. Enim in ullamco ex laboris veniam elit laborum eiusmod veniam veniam ex. Consectetur cupidatat qui laborum laborum cillum dolore minim. Tempor laborum aliquip qui consequat. Et ex nulla occaecat nulla mollit reprehenderit voluptate labore est dolore.</p>
	<br>
	<p class="text-md text-left">Duis nisi non occaecat esse magna voluptate sunt eiusmod est veniam excepteur non ullamco eiusmod. Tempor enim consectetur sit sint dolor ad cupidatat minim. Non ad reprehenderit aliquip aute esse exercitation aute sint reprehenderit ut do culpa eiusmod.</p>
	<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} darkMode={"true"} />
	<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} />
</Card>

<Form label="HenloWorld" onSubmit={() => console.log("Form Submitted")}>
	<TextField label={"Hello World"} onChange={(newValue) => console.log(newValue)} />
	<TextField label={"Hello World"} onChange={(newValue) => console.log(newValue)} />
	<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} darkMode={"true"} />
</Form>

<Accordion duration={500} />

<Code {codes} />