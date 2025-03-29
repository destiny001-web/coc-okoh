<script>
	import Title from "../../Texts/Title.svelte";


	import Bullet from "../utilities/Bullet.svelte";

    const evangelismBg = "auth/auth.png"

</script>
<section class="grid place-items-center gap-20 mt-30">
    <div class="space-y-3">
        <Title text = "Evangelism" />
        <p>Join us in spreading God's love through community outreach, charity, and missions. Be the hands and feet of Christ in a world that needs hope. As we utilize the various evangelism methods. You can participate by sending us a message.</p>
        <div class="flex flex-col gap-2">
            <div class="flex gap-2"><Bullet /> <p>House 2 House</p></div>
            <div class="flex gap-2"><Bullet /> <p>Whatsapp</p></div>
            <div class="flex gap-2"><Bullet /> <p>Radio</p></div>
            <div class="flex gap-2"><Bullet /> <p>Youtube</p></div>
            <div class="flex gap-2"><Bullet /> <p>Facebook</p></div>
        </div>
    </div>
    <div style={`background-image: url(${evangelismBg});`} class="bg-cover bg-center size-100"></div>
</section>