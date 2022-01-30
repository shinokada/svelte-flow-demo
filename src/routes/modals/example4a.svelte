<script>
	import { SmallModal, ModalButton } from '@codewithshin/svelte-flow';

	const btnName1 = 'Small Modal';
	const btnName2 = 'Small Modal 2';
	const btnSimpleName = 'Basic Modal';
	const btnColor1 = 'purple';
	const btnColor2 = 'red';
	const textSColor = 'gray';
	const id1 = 'small-modal';
	const id2 = 'small-modal-2';
	const idBasic = 'basic-modal';

	const openSmallModal1 = () => {
		toggleModal(id1);
	};

	const openSmallModal2 = () => {
		toggleModal(id2);
	};

	const openBasicModal = () => {
		toggleModal(idBasic);
	};

	const handlebtnS1 = () => {
		toggleModal(id1, false);
	};

	const handlebtnS2 = () => {
		toggleModal(id1, false);
	};

	const handlebtnS3 = () => {
		toggleModal(id2, false);
	};

	const handlebtnS4 = () => {
		toggleModal(id2, false);
	};
</script>

<div class="block p-8 space-y-4 md:space-x-4">
	<!-- Simple  -->
	<ModalButton id={idBasic} btnName={btnSimpleName} openFnName={openBasicModal} />
</div>

<SmallModal id={idBasic} title={'Basic Modal Title'}>
	<p class="text-base leading-relaxed text-{textSColor}-500 dark:text-{textSColor}-400">
		Basic Modal Content
	</p>
</SmallModal>
