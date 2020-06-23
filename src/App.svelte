<script>
	import AppBar from "./components/AppBar.svelte";
</script>

<AppBar title={{ label: "Hello World", onClick: () => console.log("Hello World") }} navLinks={[{label: "Link1", route: "/"}, {label: "Link2", route: "/"}, {label: "Link3", route: "/"}]}/>