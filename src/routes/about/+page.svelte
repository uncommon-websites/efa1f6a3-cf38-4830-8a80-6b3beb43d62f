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
			title: "Innovation",
			description: "Constantly challenging the status quo to create better solutions."
		},
		{
			title: "Integrity",
			description: "Building trust through transparent actions and honest communication."
		},
		{
			title: "Impact",
			description: "Measuring our success by the positive change we create for our clients."
		}
	];
</script>

<SecondaryHero
  title="AI dispatching for home services"
  subtitle="Increase sales and efficiency with smart recommendations and hands-on support from real people"
  imageSrc="/generated/image-a-diverse-team-collaborating-in-a-contem.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"For years, our team sat in dispatch chairs across HVAC, plumbing, electrical, and sewer companies—juggling phone calls, looking at drive times, wondering which tech would flip the job. One of those days, George Eliadis, now our CEO, asked a dispatcher why they’d picked one tech over another. The answer? ‘Just a gut feeling.’ He knew then there had to be a better way.",
		"Probook was built to replace that gut feeling with smart, data-backed decisions. From those early days at the board, we designed software to answer dispatchers’ real-world questions: Who’s closest? Who sells best? Who can get there on time? We founded Probook with a simple goal: to make dispatching easier, faster, and far more profitable. It's AI-powered, but human-first—with George often onsite during your launch, training dispatchers in person and staying until everything works.",
		"Today, Probook helps teams schedule with confidence, flip more jobs, and manage 20–25+ techs with ease. ServiceTitan syncs in real time. Customer support picks up fast. Weekly check-ins are the norm. When people ask what it feels like to work with us, one customer put it best: ‘Feels like the dispatch board finally works with me, not against me.’ That’s why we built Probook. And that’s who we built it for."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
  stakeholderType="team"
  title="Leadership"
  subtitle="Built by dispatchers, for dispatchers."
  stakeholders={[
    {
      name: "George Eliadis",
      position: "CEO",
      bio: "George is personally involved in every launch, supporting dispatchers onsite and ensuring Probook delivers real results for home services teams. His leadership blends relentless product focus with first-hand empathy for the people who use it.",
      image: "/generated/image-a-professional-headshot-of-a-male-tech-f.webp"
    }
  ]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Backed by the best."
	subtitle="Point Nine, TSIC and others"
	stakeholders={[
		{
			name: "Point Nine Capital",
			image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
		},
		{
			name: "TSIC Ventures",
			image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
		},
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to collaborate?"
	subtitle="Let's create something amazing"
	description="Join the companies already leveraging our expertise to transform their digital presence and achieve their business goals."
/>
