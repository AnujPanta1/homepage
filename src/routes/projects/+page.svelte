<script>
    import { fly } from "svelte/transition";
    import LargeWrapper from "$lib/components/LargeWrapper.svelte";
    import Section from "$lib/components/Section.svelte";
    import InfoCard from "$lib/components/ProjectSection/ProjectInfoSection.svelte";
</script>

<div in:fly={{ y: 50, duration: 500, delay: 500 }} class="m-0 h-0">
    <LargeWrapper title="Projects" color="text-blue-600">
        <div class="px-4 py-2">
            <Section title="Websites">
                <div class="my-2 flex-col gap-2 md:flex md:flex-row">
                    <InfoCard
                        title="Youtube Ripper"
                        mainText="I believe media should be free, and mp3 are alwyas fun to have ! You can search any youtube video and download a mp3 file."
                        githubLink="https://github.com/AnujPanta1/youtubeRipperv2"
                        projectLink="https://ourmusicalstorage.vercel.app/"
                        tags={["SvelteKit", "Tailwindcss", "Express", "FFMPEG"]}
                    ></InfoCard>
                    <InfoCard
                        title="Daily Poll"
                        mainText="This was a website where I used Firebase and React to create a simple site where users can answer a daily poll, and submit their own questions."
                        githubLink="https://github.com/AnujPanta1/thedailypoll"
                        projectLink="https://anujpanta1.github.io/thedailypoll/"
                        tags={["React", "Framer Motion", "Express", "Firebase"]}
                    ></InfoCard>
                    <InfoCard
                        title="Quack Quack"
                        mainText="This was a bug tracking service that I created with Subapase React and MaterialUI. It was a great practice in working on service based full stack project."
                        githubLink="https://github.com/AnujPanta1/quack-quack"
                        projectLink="https://anujpanta1.github.io/quack-quack/"
                        tags={["React", "Material UI", "Express", "Firebase"]}
                    ></InfoCard>
                </div>
            </Section>

            <Section title="Simulations">
                <div class="my-2 flex-col gap-2 sm:flex sm:flex-row">
                    <InfoCard
                        title="Friendly Fish"
                        mainText="For my Planetary Simulations class I created a final project combining multiple simulation methods to create what I called 'Friendly Fish' ! Utilizing inverse kenematics, flocking algorithims, and perlin noise fields I was able to create a beautiful animation of fish. I used parts of that projects for this websites background as well."
                        githubLink="/"
                        projectLink="/"
                        tags={[
                            "p5.js",
                            "Boid Flocking",
                            "Inverse Kenimatics",
                            "Perlin Noise",
                        ]}
                    ></InfoCard>
                    <InfoCard
                        title="Physarum Slime"
                        mainText="After reading a paper on Physarum slime written by Jeff Jones I decided to make a moving Agent simulation drawing on characteristics as written in the paper. The Agents move fully autonomously, like Physarum, around their environment moving based on the trail of other Agents."
                        githubLink="/"
                        projectLink="/"
                        tags={["Processing", "Natural Simulations"]}
                    ></InfoCard>
                </div>
            </Section>

            <Section title="other">
                <div class="my-2 flex-col gap-2 sm:flex sm:flex-row">
                    <InfoCard
                        title="The Sad Thumb of the Short Man"
                        mainText="As man that looks at himself as a short king, I decided to see if short men go through stguggles that can be hilighted with data. I decided to otulize Python and basic data and ml pattersn to analyze over 3 men's heights and their thumb size. After layres of processing, I found shorter men have small thumbs leading to a hard time buying gloves. This saddens me, but also maeks my happy that code can find things. Yay."
                        githubLink="/"
                        projectLink="/"
                        tags={["Data Stuff", "Comedy"]}
                    ></InfoCard>
                </div>
            </Section>
        </div>

        <a
            href="https://www.github.com/anujpanta1"
            target="_blank"
            class="mx-auto mb-2 flex w-fit items-center gap-3 px-4"
        >
            <p class="w-fit text-sm font-semibold text-gray-600">
                Gheck out my saucy github !
            </p>
            <svg
                xmlns="http://www.w3.org/2000/svg"
                class="icon icon-tabler icon-tabler-brand-github-filled"
                width="16"
                height="16"
                viewBox="0 0 24 24"
                stroke-width="1"
                stroke="#2c3e50"
                fill="none"
                stroke-linecap="round"
                stroke-linejoin="round"
            >
                <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                <path
                    d="M5.315 2.1c.791 -.113 1.9 .145 3.333 .966l.272 .161l.16 .1l.397 -.083a13.3 13.3 0 0 1 4.59 -.08l.456 .08l.396 .083l.161 -.1c1.385 -.84 2.487 -1.17 3.322 -1.148l.164 .008l.147 .017l.076 .014l.05 .011l.144 .047a1 1 0 0 1 .53 .514a5.2 5.2 0 0 1 .397 2.91l-.047 .267l-.046 .196l.123 .163c.574 .795 .93 1.728 1.03 2.707l.023 .295l.007 .272c0 3.855 -1.659 5.883 -4.644 6.68l-.245 .061l-.132 .029l.014 .161l.008 .157l.004 .365l-.002 .213l-.003 3.834a1 1 0 0 1 -.883 .993l-.117 .007h-6a1 1 0 0 1 -.993 -.883l-.007 -.117v-.734c-1.818 .26 -3.03 -.424 -4.11 -1.878l-.535 -.766c-.28 -.396 -.455 -.579 -.589 -.644l-.048 -.019a1 1 0 0 1 .564 -1.918c.642 .188 1.074 .568 1.57 1.239l.538 .769c.76 1.079 1.36 1.459 2.609 1.191l.001 -.678l-.018 -.168a5.03 5.03 0 0 1 -.021 -.824l.017 -.185l.019 -.12l-.108 -.024c-2.976 -.71 -4.703 -2.573 -4.875 -6.139l-.01 -.31l-.004 -.292a5.6 5.6 0 0 1 .908 -3.051l.152 -.222l.122 -.163l-.045 -.196a5.2 5.2 0 0 1 .145 -2.642l.1 -.282l.106 -.253a1 1 0 0 1 .529 -.514l.144 -.047l.154 -.03z"
                    stroke-width="0"
                    fill="currentColor"
                />
            </svg>
        </a>
    </LargeWrapper>
</div>
