<script>
    import LargeWrapper from "$lib/components/LargeWrapper.svelte";
    import Section from "$lib/components/Section.svelte";
    import { fly } from "svelte/transition";
</script>

<div in:fly={{ y: 50, duration: 500, delay: 500 }} class="h-0 m-0">
    <LargeWrapper title="Blog" color="text-purple-600">
        <div class="px-4 py-2">
            <Section title="01/03/2024">
                <div>
                    <div
                        class="text-left py-3 px-5 rounded-lg hover:bg-stone-200/80 duration-300 text-sm"
                    >
                        <p class="text-purple-600 font-semibold">
                            Simple WebDevelopment is King
                        </p>
                        <p class="text-gray-600 my-2">
                            Svelte is the best web framework, after testing it's
                            close relation to HTML CSS & JS shines. <br />
                            <br />Simple Web Development is King In the
                            ever-evolving landscape of web development, a
                            multitude of tools and frameworks promise to make
                            the job of creating websites and applications
                            easier, faster, and more efficient. Amidst this sea
                            of technology, one framework stands out for its
                            simplicity and close alignment with the core pillars
                            of web development: HTML, CSS, and JavaScript. This
                            framework is Svelte. Svelte: The Game-Changer in Web
                            Frameworks At its heart, Svelte is a radical
                            departure from traditional web frameworks. <br />
                            <br /> It's not just a library or a set of tools; it's
                            a new way of thinking about how we create web applications.
                            Svelte shifts work to compile time, converting your components
                            into highly efficient imperative code that updates the
                            DOM. This approach results in faster applications and
                            a greatly simplified coding process.
                        </p>
                    </div>
                </div>
            </Section>
        </div>
    </LargeWrapper>
</div>
