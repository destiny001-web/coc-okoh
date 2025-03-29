<script lang="ts">
	let { children } = $props();
</script>

<div class="@container overflow-hidden">
    <div class="grid gap-5 place-items-center @3xl:grid-cols-2">
        <div>
            <img src="/auth/auth.png" alt="">
        </div>
        <div>{@render children()}</div>
    </div>
</div>
