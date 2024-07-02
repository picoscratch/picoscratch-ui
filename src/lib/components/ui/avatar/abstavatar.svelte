<script lang="ts">
  import * as Avatar from "$lib/components/ui/avatar/index.js";

	export let src = "";
	export let fallback = ". . .";

	// Just the first char of each word in the fallback
	const short = fallback
		.split(" ")
		.map((word) => word[0])
		.join("").toUpperCase();
</script>
 
<Avatar.Root>
  <Avatar.Image {src} alt={fallback} />
  <Avatar.Fallback>{short}</Avatar.Fallback>
</Avatar.Root>
