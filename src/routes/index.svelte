<script >
let count =0;
function upcount(){
	count += 1;
}
function downcount(){
	count -= 1;
}
</script>

{#if count ==1 }
	<h1>
		i have {count} dollor
	</h1>
{:else}
	<h1>
		i have {count} dollors
	</h1>
{/if}

<button on:click={upcount}>
	+1
</button>
<button on:click={downcount}>
	-1
</button>