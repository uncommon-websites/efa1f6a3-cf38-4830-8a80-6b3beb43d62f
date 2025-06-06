<script lang="ts">
	// Types

	// Components
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Card from "$lib/components/ui/Card.svelte";
	import JobList, { type JobOpening } from "./JobList.svelte";

	// Icons
	import IconBriefcase from "~icons/lucide/briefcase";
	import IconUsers from "~icons/lucide/users";
	import IconHeart from "~icons/lucide/heart";
	import IconGlobe from "~icons/lucide/globe";

	// Constants
	const SECTION_BASE_CLASSES = "section-py section-px container mx-auto";
	const GRADIENT_BG_CLASSES =
		"bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-800";
	const ICON_CONTAINER_CLASSES =
		"bg-primary-50 text-primary-600 dark:bg-primary-950 dark:text-primary-400 flex items-center justify-center rounded-full";

	const benefits = [
		{
			title: "Flexible Work",
			description: "Remote-first with flexible hours that respect work-life balance.",
			icon: IconBriefcase
		},
		{
			title: "Growth Opportunities",
			description: "Continuous learning with mentorship and education stipends.",
			icon: IconUsers
		},
		{
			title: "Comprehensive Benefits",
			description: "Health coverage, retirement plans, and generous paid time off.",
			icon: IconHeart
		}
	];

	const openings: JobOpening[] = [
		// Engineering
		{
			title: "Senior Frontend Developer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Backend Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Design Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Design
		{
			title: "UX/UI Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Product
		{
			title: "Product Manager",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Analyst",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Marketing
		{
			title: "Marketing Specialist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Content Strategist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Social Media Manager",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
  {
    name: "Michael Chen",
    position: "Senior Developer",
    company: "Engineering Team",
    quote:
      "Collaboration here is the real deal—I've learned so much from teammates and we solve tough problems as a unit. There's always room to grow, and people celebrate your wins.",
    image:
      "/generated/image-a-professional-headshot-of-an-asian-male.webp"
  },
  {
    name: "Priya Sharma",
    position: "Product Designer",
    company: "Design Team",
    quote:
      "At Probook I have real ownership. My ideas turn into live features, and I get to learn from such smart, caring people—it's made me a stronger designer.",
    image:
      "/generated/image-a-professional-headshot-of-an-indian-fem.webp"
  },
  {
    name: "Marcus Johnson",
    position: "Marketing Lead",
    company: "Marketing Team",
    quote:
      "There's a clear path for growth here. Leadership supports you every step—and our team genuinely roots for each other's success.",
    image:
      "/generated/image-a-professional-headshot-of-a-black-male-.webp"
  }
];

	const processSteps = [
		{
			step: 1,
			title: "Apply",
			description: "Submit your resume and a short note about what excites you about Probook."
		},
		{
			step: 2,
			title: "Initial call",
			description: "A quick call to talk through your goals, motivations, and your questions about the team or role."
		},
		{
			step: 3,
			title: "Real-world challenge",
			description: "Complete a relevant task or walkthrough a real Probook problem to see how you think—role dependent."
		},
		{
			step: 4,
			title: "Final conversation",
			description: "Meet with our CEO or leadership for a high-level discussion on fit, ownership, and goals."
		},
		{
			step: 5,
			title: "Fast decision & onboarding",
			description: "If its a mutual match, youll get your offer fast. Start with a 2-day in-person launch alongside our team and customers."
		}
	];

	const values = [
		{
			icon: IconHeart,
			title: "Built by dispatchers, for dispatchers",
			description: "We build what matters most to real users—empathy and field-tested insight guide every feature."
		},
		{
			icon: IconUsers,
			title: "Collaboration and high trust",
			description: "We solve big problems together. Weekly team check-ins, always-on customer support, and open feedback help us learn fast and win together."
		},
		{
			icon: IconGlobe,
			title: "Relentless commitment to quality",
			description: "We take pride in our service and product. Our bar is high—for trust, innovation, and delivering results our customers rely on."
		}
	];
</script>

<!-- Hero Section -->

<SecondaryHero
	title="Empower the trades with AI"
	subtitle="Join a collaborative team building the future of dispatching—where leadership listens, customers come first, and your work makes a real impact."
	imageSrc="/generated/image-a-modern-office-setting-where-a-diverse-.webp"
/>

<!-- Why Join Us Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Why join us?" subtitle="Where empathy meets innovation and impact is real" />

	<div class="probook-why-joinus-content text-body mb-10 max-w-3xl">
		<ul class="space-y-5">
			<li><strong>Shape the product you use daily</strong> – We're built by dispatchers and home service pros, and we work hand-in-hand with users to shape the roadmap.</li>
			<li><strong>See the direct impact of your work</strong> – Our software drives major revenue growth and efficiency for every customer. You'll see exactly how your work helps teams perform better.</li>
			<li><strong>Experience world-class support</strong> – Join a team that champions partnership—not tickets. We measure success by how fast and how well we solve problems for users.</li>
			<li><strong>Grow fast with a fast-growing company</strong> – We're working with some of the top service teams in the industry—and growing quickly. There's room to move up, out, and deeper here.</li>
		</ul>
		<p class="mt-8">Every new teammate joins our hands-on, 2-day launch supporting dispatchers alongside our CEO. You’ll see our commitment to customers, innovation, and rapid growth—up close.</p>
	</div>

	<div class="mt-16 grid gap-4 md:grid-cols-3">
		{#each benefits as benefit}
			<Card {...benefit} />
		{/each}
	</div>
</section>

<!-- Culture Section -->
<Culture {values} />

<Testimonials testimonials={employeeTestimonials} />

<!-- Application Process -->
<section class={SECTION_BASE_CLASSES}>
	<div class="mx-auto">
		<h2 class="text-title1 mb-16">Our application process</h2>

		<div class="grid gap-12 md:grid-cols-3">
			{#each processSteps as { step, title, description }, i}
				<div class="flex flex-col">
					<div class="{ICON_CONTAINER_CLASSES} mb-6 size-11">
						<span class="text-headline">{step}</span>
					</div>
					<h3 class="text-headline mb-3">{title}</h3>
					<p class="text-body text-emphasis-low">{description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>
<!-- Current Openings Section -->
<section class={GRADIENT_BG_CLASSES}>
	<div class="section-px section-py container mx-auto grid w-full items-start lg:grid-cols-2">
		<SectionHeader title="Current openings" subtitle="Find your perfect role" />

		<JobList {openings} />
	</div>
</section>
