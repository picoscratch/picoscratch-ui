<script lang="ts">
    import * as Accordion from "$lib/components/ui/accordion/index.ts";
    import * as Alert from "$lib/components/ui/alert/index.ts";
    import * as Breadcrumb from "$lib/components/ui/breadcrumb/index.ts";
    import * as Card from "$lib/components/ui/card/index.ts";
    import {Avatar} from "$lib/components/ui/avatar/index.ts";
    import Badge from "$lib/components/ui/badge/badge.svelte";
    import Button from "$lib/components/ui/button/button.svelte";
    import { Description } from "$lib/components/ui/dialog/index.ts";
		// import * as Dialog from "$lib/components/ui/dialog/index.ts";
    import Switch from "$lib/components/ui/switch/switch.svelte";
    import Checkbox from "$lib/components/ui/checkbox/checkbox.svelte";
	import "../app.css";
	// import { onMount } from "svelte";

	// let isDesktop = true;

	// let Thing: typeof Dialog | typeof Drawer = Dialog;
	// let ThingRoot: typeof Dialog.Root | typeof Drawer.Root = Dialog.Root;
	// let ThingTrigger: typeof Dialog.Trigger | typeof Drawer.Trigger = Dialog.Trigger;
	// let ThingContent: typeof Dialog.Content | typeof Drawer.Content = Dialog.Content;
	// let ThingHeader: typeof Dialog.Header | typeof Drawer.Header = Dialog.Header;
	// let ThingTitle: typeof Dialog.Title | typeof Drawer.Title = Dialog.Title;
	// let ThingDescription: typeof Dialog.Description | typeof Drawer.Description = Dialog.Description;
	// let ThingFooter: typeof Dialog.Footer | typeof Drawer.Footer = Dialog.Footer;

	// onMount(() => {
	// 	isDesktop = innerWidth > 768;
	// 	// Thing = Drawer;
	// 	ThingRoot = Drawer.Root;
	// 	ThingTrigger = Drawer.Trigger;
	// 	ThingContent = Drawer.Content;
	// 	ThingHeader = Drawer.Header;
	// 	ThingTitle = Drawer.Title;
	// 	ThingDescription = Drawer.Description;
	// 	ThingFooter = Drawer.Footer;
	// })
</script>
<h1>Welcome to your library project</h1>
<p>Create your package using @sveltejs/package and preview/showcase your work with SvelteKit</p>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<Button>THIS IS A BUTTON</Button>
<Button variant="secondary">This is a secondary button</Button>
<Button variant="destructive">THIS IS A DESTRUCTIVE BUTTON</Button>

<Switch checked />
<Checkbox checked="indeterminate" />

<Alert.Root variant="destructive">
	<svg width="24" height="24" fill="none" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M10.876 8.661c.387.216.848.339 1.37.339.847 0 1.555-.307 2.047-.844.481-.526.703-1.216.703-1.906a.75.75 0 0 0-1.5 0c0 .377-.12.686-.31.894-.18.196-.472.356-.94.356-.449 0-.73-.162-.914-.37A1.46 1.46 0 0 1 11 6.29V4.25A2.25 2.25 0 0 1 13.25 2h3.185c.509 0 1.007.141 1.44.408l2.768 1.703A.75.75 0 0 1 21 4.75v1.5a2.25 2.25 0 0 1-2.25 2.25h-.25v9.533c.92.088 1.618.366 2.047.964.257.359.36.76.408 1.129.045.352.045.736.045 1.09v.034a.75.75 0 0 1-.75.75h-3.252v-.774c0-.572.002-2.208-1.5-3.169v-2.804a.75.75 0 0 0-1.5 0v2.266a4.622 4.622 0 0 0-.697-.022c-.026 0-.049.002-.064.003h-.025l-.003.001a.75.75 0 1 0 .082 1.498h.003l.013-.001.05-.002c.041-.002.093-.003.141-.003.432 0 .715.073.901.17l.033.017c1.039.484 1.066 1.439 1.066 2.07V22H5.833a3.833 3.833 0 0 1-1.97-7.123.75.75 0 0 1 .772 1.287A2.333 2.333 0 0 0 5.833 20.5c.319 0 .517-.083.649-.176.139-.098.248-.238.331-.407a1.928 1.928 0 0 0 .187-.69v-.035l.004-.143a14.198 14.198 0 0 1 .26-2.187c.26-1.291.797-2.968 1.952-4.139.848-.86 1.309-2.119 1.547-3.364.046-.238.083-.472.113-.698Z" fill="#ffffff"/></svg>
	<Alert.Title>Alert Title</Alert.Title>
	<Alert.Description>
		Alert Description
	</Alert.Description>
</Alert.Root>

<Accordion.Root class="w-full sm:max-w-[70%]">
  <Accordion.Item value="item-1">
    <Accordion.Trigger>Is it cool?</Accordion.Trigger>
    <Accordion.Content
      >Yes.</Accordion.Content
    >
  </Accordion.Item>
  <Accordion.Item value="item-2">
    <Accordion.Trigger>Accordion Title</Accordion.Trigger>
    <Accordion.Content>
      Accordion Content
    </Accordion.Content>
  </Accordion.Item>
  <Accordion.Item value="item-3">
    <Accordion.Trigger>Accordion Title 2</Accordion.Trigger>
    <Accordion.Content>
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt aperiam, nisi voluptatem repellat consequatur beatae natus error voluptates officia officiis placeat repellendus! Optio numquam repellat veniam nam libero quae sequi.
    </Accordion.Content>
  </Accordion.Item>
</Accordion.Root>

<Avatar src="https://avatars.githubusercontent.com/u/58847300" fallback="Melt UI" />

<Badge>Badge</Badge>
<Badge variant="destructive">Badge</Badge>
<Badge variant="outline">Badge</Badge>

<Breadcrumb.Root>
  <Breadcrumb.List>
    <Breadcrumb.Item>
      <Breadcrumb.Link href="/">Home</Breadcrumb.Link>
    </Breadcrumb.Item>
    <Breadcrumb.Separator />
    <Breadcrumb.Item>
			<Breadcrumb.Link href="/docs">Docs</Breadcrumb.Link>
    </Breadcrumb.Item>
    <Breadcrumb.Separator />
    <Breadcrumb.Item>
      <Breadcrumb.Link href="/docs/components">Components</Breadcrumb.Link>
    </Breadcrumb.Item>
    <Breadcrumb.Separator />
    <Breadcrumb.Item>
      <Breadcrumb.Page>Breadcrumb</Breadcrumb.Page>
    </Breadcrumb.Item>
  </Breadcrumb.List>
</Breadcrumb.Root>

<Card.Root class="w-[350px]">
  <Card.Header>
    <Card.Title>Card</Card.Title>
    <Card.Description>This is a card.</Card.Description>
  </Card.Header>
  <Card.Content>
		Content!
  </Card.Content>
  <Card.Footer class="justify-end gap-2">
    <Button variant="outline">Cancel</Button>
    <Button>OK</Button>
  </Card.Footer>
</Card.Root>