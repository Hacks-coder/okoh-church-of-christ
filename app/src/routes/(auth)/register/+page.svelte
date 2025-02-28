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
        <Title text = "Create An Account" />
        <div class="bg-dullgold w-80 rounded-xl px-3 flex gap-2 items-center shadow-xs shadow-black">
            <IconEmail class="text-xl text-gold"/>
            <input type="email" placeholder="Enter your email" required class="bg-transparent focus:outline-none h-10 w-70 placeholder:text-black">
        </div>
        <div class="bg-dullgold w-80 rounded-xl px-3 flex gap-2 items-center shadow-xs shadow-black">
            <IconPassword class="text-xl text-gold"/>
            <input type="password" placeholder="Enter your password" required class="bg-transparent focus:outline-none h-10 w-70 placeholder:text-black">
            <IconEyeClosed class="text-xl text-gold"/>
        </div>
        <div class="flex gap-2">
            <input type="checkbox" class="checked:text-gold">
            <small>I agree to the <span class="text-gold font-bold">Terms & Conditions</span> and <span class="text-gold font-bold"> Privacy policies</span></small>
        </div>
        <Fill text = "Sign in" />
        <small>or sign-up with</small>
        <Auth />
        <small>I already have an account. <a href="/login" class="text-gold">Sign-in</a></small>
    </form>
</div>