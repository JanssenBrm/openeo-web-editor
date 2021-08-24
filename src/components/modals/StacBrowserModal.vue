<template>
	<Modal title="Batch Job Result" @closed="$emit('closed')">
		<StacBrowser catalogUrl="https://raw.githubusercontent.com/cholmes/pdd-stac/beta2/disasters/collection.json" />
	</Modal>
</template>

<script>
import Modal from './Modal.vue';
import StacBrowser from '@radiantearth/stac-browser/src/StacBrowser.vue';

export default {
	name: 'StacBrowserModel',
	components: {
		Modal,
		StacBrowser
	}
}
</script>