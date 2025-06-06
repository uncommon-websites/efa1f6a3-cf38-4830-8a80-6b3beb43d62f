<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
	title="Every phone call, perfectly dispatched"
	subtitle="The fastest way to assign the right tech, boost revenue, and run a smoother board."
	centered={false}
	customers={[
		{
			name: "Jessica Lee",
			position: "Senior HVAC Dispatcher, AirNow Services",
			imageSrc: "/generated/image-a-female-hvac-dispatcher-in-an-office-en.webp"
		},
		{
			name: "David Martinez",
			position: "Operations Manager, Precision Plumbing",
			imageSrc: "/generated/image-a-confident-male-plumbing-company-manage.webp"
		},
		{
			name: "Emily Chen",
			position: "Lead Electrical Tech, BrightCurrent Electric",
			imageSrc: "/generated/image-a-female-electrical-technician-holding-a.webp"
		},
		{
			name: "Tyrone Jenkins",
			position: "Sewer Services Supervisor, JetClean Utilities",
			imageSrc: "/generated/image-a-male-sewer-services-supervisor-onsite-.webp"
		},
		{
			name: "Sarah Thompson",
			position: "Dispatch Coordinator, HomeWorks Pros",
			imageSrc: "/generated/image-a-female-home-services-dispatcher-at-her.webp"
		}
	]}
	callsToAction={[
		{ href: "/demo", label: "Book a demo" },
		{ href: "/how-it-works", label: "How it works" }
	]}
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		"https://logo.clearbit.com/ars.com",
		"https://logo.clearbit.com/reliantairconditioning.com",
		"https://logo.clearbit.com/servicechampions.net",
		"https://logo.clearbit.com/riversideelectrical.com"
	]}
/>

<Summary
	title="AI dispatching, for home services."
	text="Probook is AI-powered dispatching software built for HVAC, plumbing, electrical, and sewer service teams. Assign the right technician to every job, increase sales, and run a smoother board—without burning out your dispatchers."
/>

<Testimonials
	testimonials={[
		{
			name: "Maria Alvarez",
			position: "Office Manager, AquaPure Plumbing",
			company: "AquaPure Plumbing",
			quote:
				"With Probook, we cut our job assignment process in half. I spend less time stressing over schedules and more time helping our techs succeed. We see fewer mistakes and a lot less overtime. Probook just makes everything smoother and more predictable—my team loves it!",
			image: "/generated/image-a-latina-woman-dressed-in-smart-business.webp"
		},
		{
			name: "Malik Carter",
			position: "Lead Dispatch, Unity HVAC",
			company: "Unity HVAC",
			quote:
				"Every week we save thousands. Probook’s AI means jobs are matched instantly and our best techs always land the top calls. It’s made a huge difference for our revenue and finally lets me step away from emergency decisions. Our risk of missed sales and unnecessary drive time is way down.",
			image: "/generated/image-a-black-man-wearing-a-tidy-hvac-technici.webp"
		},
		{
			name: "Eric Zhu",
			position: "Operations Coordinator, Lumin Electrical",
			company: "Lumin Electrical",
			quote:
				"I used to juggle schedules day and night, but Probook’s smart dispatching lets me plan weeks ahead. We're saving money on fuel and payroll, and my time goes to building the business, not putting out fires. I’ve never trusted a software more to keep my team—and me—on track.",
			image: "/generated/image-an-asian-man-in-an-electrical-company-wa.webp"
		}
	]}
/>

<Features
	title="AI dispatching that boosts your bottom line"
	subtitle="Probook uses AI to send the right tech to the right job, increasing sales, lowering drive time, and scaling your team’s output with less stress."
	features={[
		{
			title: "Put your best tech on every call",
			description: "Probook analyzes performance metrics, job types, and drive times to assign the tech most likely to close and convert—proven to lift revenue per opportunity."
		},
		{
			title: "Two automation modes, one simple interface",
			description: "Use Copilot for recommendations you can control, or Autopilot to manage 20–25+ techs in real time with automated dispatching you can trust."
		},
		{
			title: "Real-time sync with ServiceTitan",
			description: "Probook creates no extra work or learning curves—every decision, job, and change instantly updates inside ServiceTitan exactly how your team expects."
		},
		{
			title: "Hands-on onboarding—CEO included",
			description: "Your team gets full onboarding support, including a 2-day in-person launch where our CEO personally helps dispatchers get confident on day one."
		},
		{
			title: "The fastest, most helpful support in the industry",
			description: "We respond in under 3 minutes, resolve issues within 25, and follow through until dispatchers give 100% satisfaction. No ticket queues. Just answers."
		},
		{
			title: "Boosted sales and efficiency, instantly",
			description: "Maximize every revenue opportunity while cutting wasted drive time, without adding workload or sacrificing trust in your dispatching decisions."
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Maximize revenue per call",
			description: "Probook sends your strongest techs to the highest-value opportunities—so you sell more without adding headcount.",
			image: "/generated/image-a-friendly-hvac-technician-with-a-tool-b.webp",
			link: {
				href: "/use-cases/maximize-revenue",
				label: "Learn more"
			}
		},
		{
			title: "Cut drive time and overtime",
			description: "Our AI minimizes mileage while fully using your workforce—helping you serve more customers, with fewer wasted hours.",
			image: "/generated/image-a-group-of-hvac-technicians-in-a-parking.webp",
			link: {
				href: "/use-cases/reduce-drive-time",
				label: "Learn more"
			}
		},
		{
			title: "Onboard dispatchers 10x faster",
			description: "New dispatchers rely on clear recommendations instead of memorizing tech stats or coverage maps.",
			image: "/generated/image-in-an-office-setting-a-dispatcher-is-war.webp",
			link: {
				href: "/use-cases/fast-onboarding",
				label: "Learn more"
			}
		}
	]}
/>

<AboutTeaser />
<CallToAction
  title="Smarter dispatching. Higher profits."
  subtitle="One AI platform. More sales, less stress."
  description="Probook uses AI to connect the best tech to every job—automatically. Boost revenue, cut drive time, and grow without adding new headcount. Rapid onboarding, live support, and instant ServiceTitan sync—all with results you can see in the first week."
  imageSrc="/generated/image-a-cheerful-dispatcher-or-office-manager-.webp"
  callsToAction={[{ href: '/demo', label: 'Book a demo', variant: 'primary' }, { href: '/contact', label: 'Talk to sales', variant: 'secondary' }]}
/>
