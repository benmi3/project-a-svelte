<script lang="ts">
	import { user } from './auth';
	// TODO: Add levels of permissions here
</script>

{#if $user}
	<slot name="authed"></slot>
{:else}
	<slot name="not_authed"></slot>
{/if}
