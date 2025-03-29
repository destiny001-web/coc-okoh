<script>

	import Fill from "../../Buttons/Fill.svelte";
	import Outline from "../../Buttons/Outline.svelte";

</script>
<section class="relative w-full py-10 flex items-center justify-center text-white">
    <div class="absolute inset-0 bg-cover bg-center w-full" style="background-image: url('/hero/hero.jpg');"></div>
    <div class="absolute inset-0 bg-black opacity-50"></div>
    <div class="relative z-10 text-center flex flex-col gap-5">
        <div class="flex flex-col items-center text-center">
            <div class="flex gap-2">
                <p>The Church of Christ</p>
                <div class="rounded-full size-10 border-2 border-white" style={`background-image: url($("/hero/hero.jpg"))`}></div>
                <p>Okoh</p>
            </div>
            <div class="flex gap-2">
                <div class="rounded-full h-10 w-30 border-2 border-white" style={`background-image: url($("/hero/hero.jpg"))`}></div>
                <p>Welcome You</p>
            </div>
        </div>
        <p class="text-xs">But if I tarry long, that thou mayest know how thou oughtest to behave thyself in the house of God, which is the church of the living God, the pillar and ground of the truth.</p>
        <div>
            <Fill text = "Join Us" />
            <Outline text = "Visit" />
        </div>
        <div></div>
    </div>
</section>