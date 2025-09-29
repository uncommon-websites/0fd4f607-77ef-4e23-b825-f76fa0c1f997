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
			title: "Signal over noise",
			description: "Cutting through scattered directories to surface only the most relevant exhibitions for your context."
		},
		{
			title: "Early discovery",
			description: "Spotting emerging talent and under-the-radar venues before they hit mainstream coverage."
		},
		{
			title: "Art world focus",
			description: "Built by insiders who understand the unique needs of gallery directors and collectors."
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
			bio: "Long-time art world operator who experienced firsthand the frustration of tracking meaningful exhibitions across scattered directories.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Trusted by the art community."
	subtitle="From gallery directors to serious collectors"
	stakeholders={[
		{
			name: "Gallery Directors",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Art Collectors",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Art Fair Partners",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to discover better shows?"
	subtitle="Join thousands who trust INDEX for exhibition discovery"
	description="Stop wasting time on scattered directories. Start finding the right exhibitions at the right time with location-aware search and curated artist data."
/>
