<script>
    import MyButton from '$lib/button.svelte';
    import { AccordionGroup, AccordionItem } from '@skeletonlabs/skeleton';
    let name= 'William';
    let myString = `this is a random sentence. Hello ${name}`;
</script>


<h1>hi world</h1>
<h2>{myString}</h2>
<MyButton/>


<AccordionGroup collapse={false}>
	<AccordionItem open>
		<svelte:fragment slot="lead">(icon)</svelte:fragment>
		<svelte:fragment slot="summary">(summary)</svelte:fragment>
		<svelte:fragment slot="content">(content)</svelte:fragment>
	</AccordionItem>
	<AccordionItem>
		<svelte:fragment slot="lead">(icon)</svelte:fragment>
		<svelte:fragment slot="summary">(summary)</svelte:fragment>
		<svelte:fragment slot="content">(content)</svelte:fragment>
	</AccordionItem>
	<!-- ... -->
</AccordionGroup>


<style>
    h1 {
        font-size: 51px !important;
    }
</style>

