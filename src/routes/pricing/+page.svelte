<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
	testimonials={[
  {
    name: "Nicole Baptiste",
    position: "Dispatcher",
    company: "HeatWorx HVAC",
    quote:
      "We flipped more leads and had fewer no-sales weeks within the first month of using Probook. Average ticket is up 16%. Training our team took less than a day—super simple.",
    image:
      "/generated/image-a-confident-black-woman-dispatcher-dress.webp"
  },
  {
    name: "Luis Mendieta",
    position: "Dispatch Lead",
    company: "3 Rivers Plumbing",
    quote:
      "I run 23 techs easily—sometimes I don’t even touch the board. The AI’s recommendations grew our sales per tech by 18%. The ROI is obvious.",
    image:
      "/generated/image-a-latino-man-in-a-crisp-work-uniform-is-.webp"
  },
  {
    name: "Tariq Sayeed",
    position: "General Manager",
    company: "Oregon Electric Pro",
    quote:
      "We were wasting time assigning the wrong jobs to the wrong people. Probook cut tech drive time by 22% and our dispatchers are less stressed than ever.",
    image:
      "/generated/image-a-middle-eastern-man-wearing-a-smart-cas.webp"
  }
]}
/>

<CallToAction
  title="Smarter dispatching. Less guesswork."
  subtitle="Built by dispatchers, for dispatchers"
  description="Probook makes home service dispatching faster, easier, and more profitable—without adding headcount. Send the right tech to every job, reduce drive times, and win more flips using real-time data and AI recommendations. See results in weeks, not months, with hands-on launch support from our team."
  imageSrc="/generated/image-a-cheerful-home-services-dispatcher-sitt.webp"
  callsToAction={[
    { href: 'https://calendly.com/george-eliadis/probook-demo', label: 'Book a demo', variant: 'primary' },
    { href: 'mailto:support@probook.ai', label: 'Talk to the team', variant: 'secondary' }
  ]}
/>
