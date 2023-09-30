<script>
	import Navbar from '$lib/Navbar.svelte';
	import ContactVector from '$lib/sub-components/ContactVector.svelte';
</script>

<Navbar />

<div class="overflow-hidden">
	<ContactVector />

	<div
		class="h-screen xl:w-screen hero text-white px-[3.125rem] xl:px-[12.125rem] z-[10] relative flex flex-col justify-center gap-[3.75rem]"
	>
		<div class="contact-header text-[3rem] font-semibold">Contatct Us</div>

		<div class="flex justify-center h-fit">
			<div class="w-[40%] contact-info flex flex-col gap-[1.875rem]">
				<div class="email flex flex-col gap-[0.875rem]">
					<div class="text-[0.875rem] opacity-50">Send us an Email</div>
					<div class="text-[1.125rem] font-semibold">
						<a href="mailto:Hello@mafflestudio.com">Hello@mafflestudio.com</a>
					</div>
				</div>
				<div class="phone flex flex-col gap-[0.875rem]">
					<div class="text-[0.875rem] opacity-50">For work proposals and inquiries call</div>
					<tel class="text-[1.125rem] font-semibold">+2349070933598</tel>
				</div>
			</div>
			<div class="form flex flex-col items-center xl:gap-[3.438rem] gap-[2rem] w-[60%]">
				<div class="form-header w-full text-[1.5rem] leading-[140%]">
					Wanna start a project? Let’s talk about it
				</div>
				<div class="form-elements w-full flex flex-col xl:gap-[4.125rem] gap-[2rem]">
					<input
						type="email"
						name="email"
						id="email"
						placeholder="Your Email"
						autocomplete="email"
						class="form-input py-[10px] border-b border-b-white bg-transparent w-full focus:outline-0"
					/>
					<textarea
						placeholder="Tell us about your project"
						class="form-input py-[10px] border-b border-b-white bg-transparent w-full focus:outline-0"
						rows="1"
					/>
					<input
						type="submit"
						name="submut-button"
						id="submit"
						class="py-[0.625rem] px-[3.125rem] bg-white w-fit text-[#201F1F]"
					/>
				</div>
			</div>
		</div>
	</div>
</div>
