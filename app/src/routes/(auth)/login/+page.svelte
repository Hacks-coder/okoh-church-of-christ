<script>
    import IconEmail from '~icons/mdi/email'
    import IconPassword from '~icons/mdi/lock'
    import IconEyeClosed from '~icons/mdi/eye-off'
	import Fill from "../../../components/Buttons/Fill.svelte";
	import Auth from "../../../components/Media/Auth.svelte";
	import Title from "../../../components/Texts/Title.svelte";
</script>


<div class="bg-white p-2 w-full rounded-4xl">
    <form class="flex flex-col gap-3 text-center items-center ">
        <Title text = "Sign in Your Account" />
        <div class="bg-dullgold w-80 rounded-xl px-3 flex gap-2 items-center shadow-xs shadow-black">
            <IconEmail class="text-xl text-gold"/>
            <input type="email" placeholder="Enter your email" required class="bg-transparent focus:outline-none h-10 w-70 placeholder:text-black">
        </div>
        <div class="bg-dullgold w-80 rounded-xl px-3 flex gap-2 items-center shadow-xs shadow-black">
            <IconPassword class="text-xl text-gold"/>
            <input type="password" placeholder="Enter your password" required class="bg-transparent focus:outline-none h-10 w-70 placeholder:text-black">
            <IconEyeClosed class="text-xl text-gold"/>
        </div>
        <Fill text = "Sign in" />
        <small>or sign-in with</small>
        <Auth />
        <small>I don't have an account. <a href="/register" class="text-gold">Sign-up</a></small>
    </form>
</div>