<script>
	import "../app.postcss";
	import {
		Navbar,
		NavBrand,
		NavLi,
		NavUl,
		NavHamburger,
		DarkMode,
		Footer,
		FooterLinkGroup,
		FooterLink,
		FooterIcon,
		Button
	} from "flowbite-svelte";
	import { page } from "$app/stores";

	$: activeUrl = $page.url.pathname;
	let activeClass =
		"text-white bg-kljb-green md:bg-transparent md:text-kljb-green md:dark:text-white dark:bg-green-600 md:dark:bg-transparent";
	let nonActiveClass =
		"text-gray-700 hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-kljb-green dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent";
</script>

<div class="bg-white dark:bg-gray-900 min-h-screen m-0 flex flex-col">
	<Navbar let:hidden let:toggle class="bg-white dark:bg-gray-900">
		<NavBrand href="/">
			<img src="/KLJB-Logo-cmyk.png" class="mr-3 h-6 md:h-9" alt="KLJB Logo" />
			<span class="self-center text-xl font-semibold text-gray-700 dark:text-white">
				KLJB Kläham-Oberergoldsbach
			</span>
		</NavBrand>
		<NavHamburger on:click={toggle} />
		<div class="flex md:order-2">
			<DarkMode size="sm" />
			<!-- TODO change to flowbite icon when available -->
			<a
				href="https://www.instagram.com/kljb_klaeham/"
				class="focus:outline-none whitespace-normal m-0.5 rounded-lg focus:ring-2 p-2.5 focus:ring-gray-400 hover:bg-gray-100 dark:hover:bg-gray-600 hidden sm:inline-block dark:hover:text-white hover:text-gray-900"
				aria-label="View on Instagram"
				target="_blank"
				rel="noreferrer"
			>
				<svg class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true" role="img">
					<path
						fill-rule="evenodd"
						d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"
						clip-rule="evenodd"
					/>
				</svg>
			</a>
		</div>
		<NavUl {activeUrl} {hidden} {activeClass} {nonActiveClass} class="order-1">
			<NavLi href="/">Home</NavLi>
			<NavLi href="/become-member">Mitglied werden</NavLi>
		</NavUl>
	</Navbar>

	<section class="bg-white dark:bg-gray-900 flex-1">
		<div class="py-8 px-4 mx-auto max-w-screen-lg lg:py-16 lg:px-6">
			<slot />
		</div>
	</section>

	<Footer class="bg-white dark:bg-gray-900">
		<FooterLinkGroup
			ulClass="mx-auto flex flex-wrap items-start mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0"
		>
			<FooterLink href="imprint">Impressum</FooterLink>
			<FooterLink href="/data-protection">Datenschutz</FooterLink>
		</FooterLinkGroup>
	</Footer>
</div>
