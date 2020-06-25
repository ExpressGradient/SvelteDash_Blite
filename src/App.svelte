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
	import FloatingCard from "./components/FloatingCard.svelte";

	const codes = [
		"<h1>Hello World</h1>",
		"<p>Thanks for using SvelteDash</p>"
	];
</script>

<AppBar title={"Hello World"} navLinks={[{label: "Link1", route: "/"}, {label: "Link2", route: "/"}, {label: "Link3", route: "/"}]} on:click={() => console.log("Hello World")}/>

<RaisedButton label={"Hello World"} on:click={() => console.log("Button Clicked")} />

<RaisedButton label={"Hello World"} on:click={() => console.log("Button Clicked")} darkMode={"true"} />

<OutlineButton label={"Hello World"} on:click={() => console.log("Button Clicked")} />

<Link link={{ label: "This is a link", route: "/" }} />

<TextField label={"Hello World"} on:change={(event) => console.log(event.target.value)} />

<Card>
	<h1 class="text-3xl text-center">Hello World</h1>
	<p class="text-md text-left">Sunt dolor est elit proident laboris qui laboris. Enim in ullamco ex laboris veniam elit laborum eiusmod veniam veniam ex. Consectetur cupidatat qui laborum laborum cillum dolore minim. Tempor laborum aliquip qui consequat. Et ex nulla occaecat nulla mollit reprehenderit voluptate labore est dolore.</p>
	<br>
	<p class="text-md text-left">Duis nisi non occaecat esse magna voluptate sunt eiusmod est veniam excepteur non ullamco eiusmod. Tempor enim consectetur sit sint dolor ad cupidatat minim. Non ad reprehenderit aliquip aute esse exercitation aute sint reprehenderit ut do culpa eiusmod.</p>
	<RaisedButton label={"Hello World"} on:click={() => console.log("Button Clicked")} darkMode={"true"} />
	<RaisedButton label={"Hello World"} on:click={() => console.log("Button Clicked")} />
</Card>

<FloatingCard>
	<h1 class="text-2xl">Hello World</h1>
	<p class="text-md">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Culpa impedit inventore laboriosam maxime optio quos repudiandae sapiente, sit suscipit totam veniam voluptate voluptatem? Amet cum explicabo libero perspiciatis repudiandae. Aperiam placeat, quam. Asperiores doloribus eveniet mollitia obcaecati quas? A accusantium amet aperiam blanditiis consectetur explicabo fuga hic illum labore magnam maiores mollitia neque nisi obcaecati odio perspiciatis porro quaerat quas, qui ratione sed sit tenetur totam unde veritatis vero vitae? Architecto, obcaecati tenetur! Cum dignissimos dolorum eligendi fuga magnam maxime soluta tempora temporibus vitae. Adipisci cupiditate ducimus exercitationem illum magnam nobis saepe velit voluptates! Earum nostrum quibusdam rerum sequi sunt!</p>
</FloatingCard>

<Form label="HenloWorld" on:submit={() => console.log("Form Submitted")}>
	<TextField label={"Hello World"} on:change={(newValue) => console.log(newValue)} />
	<TextField label={"Hello World"} on:change={(newValue) => console.log(newValue)} />
	<RaisedButton label={"Hello World"} on:click={() => console.log("Button Clicked")} darkMode={"true"} />
</Form>

<Accordion title="Hello World">
	<p class="text-xl">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquam at beatae deleniti, dolor doloremque esse, ex id incidunt ipsa ipsum itaque laudantium magnam minima nesciunt nisi omnis quo repellat repellendus sequi sit ut veritatis voluptate voluptatem? Ad autem, enim eveniet id laboriosam laborum nemo recusandae, tempora tempore ut vel voluptatibus.</p>
</Accordion>

<Code {codes} />