<script>
	import CardGrid from '../../lib/components/CardGrid.svelte';
	import Navbar from '../../lib/components/Navbar.svelte';
	import ProfileSection from './ProfileSection.svelte';

    
</script>

<div class="container">
	<Navbar />
	<div class="content">
		<ProfileSection />
		<CardGrid />
	</div>
</div>

<style>
    .content {
        margin: 20px;
        display: flex;
    }
</style>