<script>
	import { fade, fly } from 'svelte/transition';
	import { scale } from 'svelte/transition';
    import MenuIcon from '~icons/heroicons-outline/menu';
    let hasNavigationBeenOpen = false;
    const toogleNavigation = () => {
        hasNavigationBeenOpen = !hasNavigationBeenOpen;
    };
    
    const navagationLinks = [
        {href: "/home", child: "Home"},
        {href: "/about", child: "About"},
        {href: "/contact", child: "Contact"},
        {href: "/courses", child: "Courses"}
    ];
</script>



<header>
    <nav class="flex justify-between">
        <div>
            <img src="/logos/logo.png" width="40" alt="">
        </div>
        <div class="3xl:hidden">
            <MenuIcon class="text-3xl text-orange" onclick={toogleNavigation}/>
            {#if hasNavigationBeenOpen}
                <div class="flex flex-col z-50 w-20 p-5 bg-gray-300 rounded-2xl"  in:fly={{ x: 200, duration: 200 }} out:fly={{ x: -200, duration: 200 }}>
                    
                    {#each navagationLinks as {href, child}}
                        <a {href} onclick={toogleNavigation}>{child}</a>
                    {/each}
                </div>
            {/if}
        </div>

        <!-- desktop links -->
        <div class="hidden gap-10 text-xl font-bold @3xl:flex">
            {#each navagationLinks as {href, child}}
                <a {href} class="hover:text-orange">{child}</a>
            {/each}
        </div>
    </nav>
</header>