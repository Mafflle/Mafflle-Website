<script>
	import Navbar from '$lib/Navbar.svelte';
	import ContactVector from '$lib/sub-components/ContactVector.svelte';
</script>

<Navbar />

<div>
	<ContactVector />

	<div class="container overflow-hidden">
		<div
			class="h-[135vh] md:h-screen xl:w-screen hero text-white px-[1rem] lg:px-[3.125rem] xl:px-[12.125rem] z-[10] relative flex flex-col justify-center gap-[3.75rem]"
		>
			<div class="contact-header text-lg md:text-[3rem] font-semibold mt-16">Contact Us</div>
			<!-- Added margin-top (mt-16) for separation -->

			<div class="flex flex-col md:flex-row justify-center h-fit gap-[4.188rem] md:gap-0">
				<div class="w-full md:w-[40%] contact-info flex flex-col gap-[1.875rem]">
					<div class="email flex flex-col gap-[0.875rem]">
						<div class="text-sm opacity-50">Send us an Email</div>
						<div class="text-[1.125rem] font-semibold">
							<a href="mailto:Hello@mafflestudio.com">Hello@mafflestudio.com</a>
						</div>
					</div>
					<div class="phone flex flex-col gap-[0.875rem]">
						<div class="text-[0.875rem] opacity-50">For work proposals and inquiries call</div>
						<tel class="text-[1.125rem] font-semibold">+2349070933598</tel>
					</div>
				</div>
				<div
					class="form flex flex-col items-center xl:gap-[3.438rem] gap-[3.75rem] md:gap-[2rem] w-full md:w-[60%]"
				>
					<div class="form-header w-full text-lg md:text-[1.5rem] leading-[140%]">
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
							rows="4"
							cols="1"
						/>
						<!-- Fix: Added closing tag for textarea -->
						<input
							type="submit"
							name="submit-button"
							id="submit"
							class="py-[0.625rem] px-[3.125rem] bg-white w-fit text-[#201F1F]"
						/>
					</div>
				</div>
			</div>
			<div
				class="footer-container block md:hidden px-[1rem] lg:px-[3.125rem] xl:px-[12.125rem] py-[2.313rem] border-t border-black"
			>
				<div
					class="footer flex flex-col md:flex-row justify-between w-full items-center gap-[1.25rem]"
				>
					<div class="copyright">Ⓒ2022 Mafflle Studio. All right reserved.</div>
					<div class="social-links flex items-center gap-[1.25rem] md:gap-[5.688rem]">
						<a href="/" class="link">Twitter</a>
						<a href="/" class="link">Linkedin</a>
						<a href="/" class="link">Instagram</a>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>
