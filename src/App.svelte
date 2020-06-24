<script>
	import AppBar from "./components/AppBar.svelte";
	import RaisedButton from "./components/RaisedButton.svelte";
	import OutlineButton from "./components/OutlineButton.svelte";
</script>

<AppBar title={{ label: "Hello World", onClick: () => console.log("Hello World") }} navLinks={[{label: "Link1", route: "/"}, {label: "Link2", route: "/"}, {label: "Link3", route: "/"}]}/>

<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} />

<RaisedButton label={"Hello World"} onClick={() => console.log("Button Clicked")} darkMode={"true"} />

<OutlineButton label={"Hello World"} onClick={() => console.log("Button Clicked")} />