<script>
    import {Navbar, NavBrand, NavHamburger, NavLi, NavUl} from "flowbite-svelte";
</script>

<Navbar>
    <NavBrand href="/">
        <img src="/photo.jpg" alt="Votre Photo" class="rounded-full w-12 h-12 object-cover shadow-lg" />
    </NavBrand>
    <NavHamburger  />
    <NavUl >
        <NavLi href="/">Home</NavLi>
        <NavLi href="/">Projects</NavLi>
        <NavLi href="/about">About</NavLi>
        <NavLi href="/contact">Contact</NavLi>
    </NavUl>
</Navbar>