<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CenteredTextOnlyHero from "$lib/components/layout/hero-sections/CenteredTextOnlyHero.svelte";

	// Icons
	import IconMapPin from "~icons/lucide/map-pin";
	import IconFilter from "~icons/lucide/filter";
	import IconRadar from "~icons/lucide/radar";
	import IconBell from "~icons/lucide/bell";
	import IconUsers from "~icons/lucide/users";
	import IconDatabase from "~icons/lucide/database";
</script>

<CenteredTextOnlyHero
	title="Discover exhibitions that matter"
	subtitle="Filter 4,000+ global shows through location-aware search. Find emerging talent before they hit mainstream directories."
	imageSrc="/generated/image-a-group-of-people-gathered-in-a-modern-n.webp"
/>
<LogoScroller
	label="Trusted by galleries and institutions"
	logoUrls={[
		'https://cdn.brandfetch.io/moma.org/w/400/h/400/logo',
		'https://cdn.brandfetch.io/gagosian.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/whitney.org/w/400/h/400/logo',
		'https://cdn.brandfetch.io/davidzwirner.com/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	generating
	testimonials={[
		{
			name: "Jane Smith",
			position: "CTO",
			company: "Tech Innovations",
			quote:
				"Their cutting-edge automation boosted our productivity by 35%.\nThe intuitive interface reduced training time and improved team adoption.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "John Doe",
			position: "Director of Operations",
			company: "Global Solutions",
			quote:
				"Their robust security protocols gave us confidence in handling sensitive data.\nThe 24/7 support team resolved issues within hours, not days.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sarah Johnson",
			position: "Product Manager",
			company: "Future Systems",
			quote:
				"The scalable platform grew seamlessly with our business needs.\nTheir customization options allowed us to tailor solutions perfectly to our workflows.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	title="Discovery platform built for the art world"
	subtitle="Transform how you find exhibitions with tools designed specifically for gallery professionals and collectors"
	features={[
		{
			title: "Location-aware discovery",
			description: "Find exhibitions by proximity with intelligent geographic filtering that surfaces shows within your preferred travel radius.",
			icon: IconMapPin,
			imageSrc: "/generated/image-a-gallery-director-thoughtfully-examinin.webp"
		},
		{
			title: "Signal-to-noise filtering",
			description: "Cut through directory clutter with curated exhibition data that eliminates irrelevant listings and focuses on quality shows.",
			icon: IconFilter,
			imageSrc: "/generated/image-an-art-curator-studying-a-collection-of-.webp"
		},
		{
			title: "Emerging talent radar",
			description: "Discover promising artists before they hit mainstream directories through our network of gallery insiders and trend analysis.",
			icon: IconRadar,
			imageSrc: "/generated/image-an-artist-focused-on-painting-at-an-ease.webp"
		},
		{
			title: "Real-time exhibition alerts",
			description: "Receive instant notifications about new shows matching your interests, ensuring you never miss important openings.",
			icon: IconBell,
			imageSrc: "/generated/image-a-well-dressed-art-collector-closely-obs.webp"
		},
		{
			title: "Curated gallery network",
			description: "Access hand-selected venues from our network of 2,500+ galleries, focusing on quality over comprehensive coverage.",
			icon: IconUsers,
			imageSrc: "/generated/image-a-series-of-interconnected-gallery-rooms.webp"
		},
		{
			title: "Clean data architecture",
			description: "Navigate exhibitions through structured artist-venue-location data that eliminates the guesswork from discovery.",
			icon: IconDatabase,
			imageSrc: "/generated/image-a-team-of-archivists-organizing-and-cata.webp"
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
