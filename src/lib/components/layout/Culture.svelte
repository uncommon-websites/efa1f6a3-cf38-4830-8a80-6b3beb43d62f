<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import { animate, stagger } from "motion";
	import { onMount } from "svelte";

	// Types
	export type Value = {
		title: string;
		description: string;
	};

	// Props
	const { values = [] }: { values: Value[] } = $props();

	let cards: HTMLElement[] = $state([]);

	onMount(() => {
		if (!cards.length) return;
		if (window.self !== window.top) return;

		animate(
			cards,
			{
				y: ["1.5rem", 0],
				filter: ["blur(2px)", "blur(0px)"],
				opacity: [0, 1]
			},
			{
				duration: 0.3,
				ease: "easeOut",
				delay: stagger(0.1, {
					ease: "easeInOut"
				})
			}
		);
	});
</script>

<section class="bg-white dark:bg-gray-950">
	<div
		class="section-py section-px container mx-auto grid gap-8 [--gap:--spacing(8)] [--radius:var(--radius-2xl)]"
	>
		<SectionHeader title="Our culture." subtitle="What drives Probook" />

		<div
			class="grid gap-(--gap)"
			style:grid-template-columns="repeat(auto-fit, minmax(280px, 1fr))"
		>
			<!-- Value: Built by dispatchers, for dispatchers -->
			<div class="relative border-t border-gray-200 pt-4 dark:border-gray-900">
				<div class="text-caption z-10">
					<div>
						<div class="text-headline mb-[1em]">Built by dispatchers, for dispatchers</div>
						<div class="text-body text-gray-500 dark:text-gray-400">We build tools we've needed ourselves—and make new dispatchers feel like pros.</div>
					</div>
				</div>
			</div>
			<!-- Value: Data you can trust -->
			<div class="relative border-t border-gray-200 pt-4 dark:border-gray-900">
				<div class="text-caption z-10">
					<div>
						<div class="text-headline mb-[1em]">Data you can trust</div>
						<div class="text-body text-gray-500 dark:text-gray-400">Every recommendation is based on real results, not gut feelings.</div>
					</div>
				</div>
			</div>
			<!-- Value: Support that never quits -->
			<div class="relative border-t border-gray-200 pt-4 dark:border-gray-900">
				<div class="text-caption z-10">
					<div>
						<div class="text-headline mb-[1em]">Support that never quits</div>
						<div class="text-body text-gray-500 dark:text-gray-400">Our team is always in your corner with industry-best speed and care.</div>
					</div>
				</div>
			</div>
			<!-- Value: Relentlessly improving -->
			<div class="relative border-t border-gray-200 pt-4 dark:border-gray-900">
				<div class="text-caption z-10">
					<div>
						<div class="text-headline mb-[1em]">Relentlessly improving</div>
						<div class="text-body text-gray-500 dark:text-gray-400">We evolve with your needs. No feature request is too small—or ignored.</div>
					</div>
				</div>
			</div>
			<!-- Value: Partnership in every call -->
			<div class="relative border-t border-gray-200 pt-4 dark:border-gray-900">
				<div class="text-caption z-10">
					<div>
						<div class="text-headline mb-[1em]">Partnership in every call</div>
						<div class="text-body text-gray-500 dark:text-gray-400">We work with both office and field teams to get every job right.</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</section>
