<script>
	import {
		Navbar,
		NavBrand,
		NavLi,
		NavUl,
		NavHamburger,
		DarkMode,
		Footer,
		FooterLinkGroup,
		FooterLink
	} from 'flowbite-svelte';
</script>

<Navbar let:hidden let:toggle>
	<NavBrand href="/">
		<img src="/KLJB-Logo-cmyk.png" class="mr-3 h-6 md:h-9" alt="KLJB Logo" />
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
			KLJB Kläham-Oberergoldsbach
		</span>
	</NavBrand>
	<NavHamburger on:click={toggle} />

	<NavUl {hidden}>
		<NavLi href="/" active={true}>Home</NavLi>
		<NavLi href="/about">Mitglied werden</NavLi>
	</NavUl>

	<DarkMode size="sm" />
</Navbar>

<Footer class="absolute bottom-0 left-0 z-20 w-full">
	<FooterLinkGroup
		ulClass="flex flex-wrap items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0"
	>
		<FooterLink href="/">Impressum</FooterLink>
		<FooterLink href="/">Datenschutz</FooterLink>
	</FooterLinkGroup>
</Footer>
