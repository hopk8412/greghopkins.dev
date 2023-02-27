<script>
	import CardGrid from '../../lib/components/CardGrid.svelte';
	import ProfileSection from './ProfileSection.svelte';
</script>

<div class="container">
	<div class="content">
		<ProfileSection />
		<CardGrid />
	</div>
</div>

<style>
    @media screen and (max-width: 600px) {
  .content {
    flex-direction: column;
}
}
    .content {
        margin: 20px;
        display: flex;
    }
</style>