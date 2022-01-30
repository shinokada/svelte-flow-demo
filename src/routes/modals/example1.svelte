<script>
	import { SmallModal, ModalButton } from '@codewithshin/svelte-flow';

	const btnBasicName = 'Basic Modal';
	const idBasic = 'basic-modal';

	const openBasicModal = () => {
		toggleModal(idBasic);
	};
</script>

<div class="block p-8 space-y-4 md:flex md:space-y-0 md:space-x-4">
	<!-- Simple  -->
	<ModalButton id={idBasic} btnName={btnBasicName} openFnName={openBasicModal} />
</div>

<SmallModal id={idBasic} title={'Basic Modal Title'}>
	<p class="text-base leading-relaxed text-gray-500 dark:text-gray-400">Basic Modal Content</p>
</SmallModal>
