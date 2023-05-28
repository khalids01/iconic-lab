<script>
	import Icon from '@iconify/svelte';
</script>

<section class="container mx-auto px-4 pb-8 pt-16">
	<h1 class="text-center mb-8 text-4xl">Login</h1>
	<div class="wrapper mx-auto bg-slate-50/5 px-6 py-8 rounded-lg max-w-sm shadow-lg">
        <form class="flex flex-col gap-4" method="POST">
			<button class="btn bg-slate-900">
				<Icon icon="skill-icons:github-light" class="text-xl flex gap-" />
				<span> Github </span>
			</button>
			<button class="btn bg-slate-800">
				<Icon icon="flat-color-icons:google" class="text-xl flex gap-" />
				<span> Google </span>
			</button>
		</form>
        <div class="flex w-full justify-between relative py-6 px-1">
            <hr class="relative z-0 w-full max-w-[150px] h-px" />
            <span class='z-10 absolute left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 text-slate-400'>or</span>
            <hr class="relative z-0 w-full max-w-[150px] h-px" />
        </div>
		<form action="?/login" method="POST">
			<label class="label mb-4">
				<input class="block !mb-4 input py-2" type="email" placeholder="mail@domain.com" />
				<!-- <div class="input-group flex"> -->

				<!-- <button type="submit" class="btn btn-sm variant-filled-primary w-auto "> Send Email </button> -->
				<!-- </div> -->
				<button type="submit" class="btn text-sm w-full variant-filled-primary w-auto">
					Send Email
				</button>
			</label>
		</form>
		
	</div>
</section>
