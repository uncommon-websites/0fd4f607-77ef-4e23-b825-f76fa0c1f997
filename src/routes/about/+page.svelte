<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Curatorial precision",
			description: "Filtering 4,000+ global exhibitions to surface only what matters to serious collectors and gallery professionals."
		},
		{
			title: "Insider intelligence", 
			description: "Early signals on emerging artists and under-the-radar venues before they hit mainstream art media."
		},
		{
			title: "Art world native",
			description: "Built by gallery insiders who understand the $67B market's unique discovery and timing challenges."
		}
	];
</script>

<SecondaryHero
	title="Find art that matters"
	subtitle="Signal over noise, always"
	imageSrc="/generated/image-a-modern-minimalist-office-environment-f.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"As a gallery director or serious collector, you shouldn't have to waste hours guessing which shows are worth your attention. But existing directories are cluttered, poorly filtered, and slow to surface new talent. You miss the right moment. Or the right artist entirely.",
		"INDEX filters over 4,000 global exhibitions with clean, structured data—artist, venue, location—so you only see what's relevant to your context. Whether you're scouting for emerging voices in Berlin or planning a trip to Mexico City, INDEX shows you what's nearby, timely, and worth seeing.",
		"Our platform doesn't wait for artists to hit the headlines. By tracking geography, timing, and under-the-radar venues, we help you spot key moves before they trickle into mainstream coverage. Less noise, more signal—because timing is everything when you're chasing the edge."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Our team."
	subtitle="Built by art world insiders who understand the discovery problem."
	stakeholders={[
		{
			name: "Lukas Amacher",
			position: "Founder",
			bio: "Art world insider who built INDEX to solve the exhibition discovery problem he faced firsthand. Background in art curation and digital platforms.",
			image: "/generated/image-a-professional-headshot-of-a-man-photogr.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Find exhibitions worth flying to"
	subtitle="Signal over noise, always"
	description="Stop wasting time on scattered directories. INDEX cuts through 4,000+ global shows with clean artist, venue, and location filters collectors actually need."
	imageSrc="/generated/image-a-diverse-group-of-people-inside-a-brigh.webp"
	callsToAction={[
		{
			href: "/",
			label: "Start exploring",
			variant: "primary"
		},
		{
			href: "/",
			label: "Get show alerts",
			variant: "secondary"
		}
	]}
/>
