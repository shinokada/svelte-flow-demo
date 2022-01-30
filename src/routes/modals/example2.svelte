<script>
	import { SmallModal, ModalButton } from '@codewithshin/svelte-flow';

	const btnName1 = 'Small Modal';
	const btnName2 = 'Small Modal 2';
	const btnColor1 = 'purple';
	const btnColor2 = 'red';
	const textSColor = 'gray';
	const id1 = 'small-modal';
	const id2 = 'small-modal-2';

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

<div class="block p-8 space-y-4 md:flex md:space-y-0 md:space-x-4">
	<ModalButton id={id1} btnName={btnName1} btnColor={btnColor1} />

	<ModalButton id={id2} btnName={btnName2} btnColor={btnColor2} />
</div>

<SmallModal
	id={id1}
	btnColor={'pink'}
	title={'Small Modal Title'}
	btn1="Yes"
	btn2="No"
	on:handlebtnS1={handlebtnS1}
	on:handlebtnS2={handlebtnS2}
>
	<p class="text-base leading-relaxed text-{textSColor}-500 dark:text-{textSColor}-400">
		Modal 1 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
		incididunt ut labore et dolore magna aliqua.
	</p>
</SmallModal>

<SmallModal
	id={id2}
	btnColor={'yellow'}
	title={'Another Small Modal Title'}
	btn1="Yes"
	btn2="No"
	on:handlebtnS1={handlebtnS3}
	on:handlebtnS2={handlebtnS4}
>
	<p class="text-base leading-relaxed text-{textSColor}-500 dark:text-{textSColor}-400">
		Modal 2 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
		incididunt ut labore et dolore magna aliqua.
	</p>
</SmallModal>
