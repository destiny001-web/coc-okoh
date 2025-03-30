<script>

	import Fill from "../../Buttons/Fill.svelte";
	import Outline from "../../Buttons/Outline.svelte";

</script>
<div class="text-center flex flex-col gap-5 mt-5 px-10 md:px-20 xl:px-30 2xl:px-40">
    <div class="flex flex-col gap-2 items-center">
        <div class="flex gap-2">
            <p class="text-xl font-bold font-title md:text-2xl xl:text-4xl 2xl:text-5xl 3xl:text-6xl">The Church of Christ</p>
            <div class="rounded-full size-10 border-2 border-white" style={`background-image: url($("/hero/hero.jpg"))`}></div>
            <p class="text-xl font-bold font-title md:text-2xl xl:text-4xl 2xl:text-5xl 3xl:text-6xl">koh</p>
        </div>
        <div class="flex gap-2">
            <div class="rounded-full h-10 w-30 border-2 border-white" style={`background-image: url($("/hero/hero.jpg"))`}></div>
            <p class="text-xl font-bold font-title md:text-2xl xl:text-4xl 2xl:text-5xl 3xl:text-6xl">Welcome You</p>
        </div>
    </div>
    <p>But if I tarry long, that thou mayest know how thou oughtest to behave thyself in the house of God, which is the church of the living God, the pillar and ground of the truth.</p>
    <div>
        <Fill text = "Join Us" />
        <Outline text = "Visit" />
    </div>
</div>