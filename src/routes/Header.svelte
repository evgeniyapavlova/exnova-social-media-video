<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import LangSwitch from '../components/LangSwitch.svelte';
</script>

<header>
	<div class="container">
		<div class="header-wrap">
			<a href="https://exnova.com/">
				<svg xmlns="http://www.w3.org/2000/svg" width="168" height="40" fill="#fff"
					><path
						d="M18.26 7.273V0h3.653v7.273h-3.652zm21.914 14.545H32.87v-3.636h7.304v3.636zm-14.922-9.532l-5.165 5.143-5.165-5.143-2.582 2.572L17.505 20l2.582-2.571L22.669 20l5.165-5.142-2.582-2.572zm-5.165 10.286l5.165 5.142 2.582-2.571L22.67 20l-2.582 2.572zm-7.748 2.57L17.505 20l2.582 2.572-5.165 5.142-2.583-2.571zm5.922 7.585V40h3.652v-7.273h-3.652zM7.304 21.818H0v-3.636h7.304v3.636zM33 4.572l-5.165 5.143 2.583 2.571 5.165-5.142L33 4.572zm-2.582 23.142l5.165 5.142L33 35.428l-5.165-5.143 2.583-2.571zM12.34 30.285l-2.583-2.571-5.165 5.142 2.583 2.572 5.165-5.143zM7.175 4.572l5.165 5.143-2.583 2.571-5.165-5.142 2.583-2.572zm50.63 13.565v-3.563h13.538v-3.665H53.565v18.183H71.47v-3.665H57.806v-3.753h12.99v-3.537h-12.99zm25.702 1.648l-3.654-3.753H74.67l6.087 6.226-6.8 6.834h5.183l4.367-4.387 4.368 4.387h5.183l-6.8-6.834 6.087-6.226h-5.183l-3.655 3.753zm12.058 9.307v-13.06h4.177v1.762c.751-1.154 2.165-2.143 4.776-2.143 5.348 0 7.297 3.031 7.297 7.177v6.264h-4.177v-6.264c0-2.168-.905-3.981-3.948-3.981s-3.948 1.813-3.948 3.981v6.264h-4.177z"
					/><path
						fill-rule="evenodd"
						d="M123.325 29.472c6.087 0 9.194-2.827 9.194-6.91 0-4.108-3.107-6.91-9.194-6.91s-9.195 2.802-9.195 6.91c0 4.083 3.108 6.91 9.195 6.91zm0-3.195c-3.604 0-5.018-1.572-5.018-3.715s1.414-3.715 5.018-3.715 5.017 1.572 5.017 3.715-1.413 3.715-5.017 3.715z"
					/><path
						d="M146.983 16.032h4.406l-7.106 13.06h-4.177L133 16.032h4.406l4.788 8.85 4.789-8.85z"
					/><path
						fill-rule="evenodd"
						d="M152.031 25.149c0 3.093 2.916 4.247 6.685 4.247 2.942 0 4.356-.811 5.094-2.016v1.712H168V21.04c0-3.55-1.605-5.388-7.272-5.388-2.445 0-4.266.33-5.539.646-.739.19-1.375.406-1.91.647l1.451 2.65c.472-.165.994-.304 1.592-.431a19.888 19.888 0 0 1 4.152-.444c2.941 0 3.349.85 3.349 2.003-6.94-.507-11.792.127-11.792 4.426zm4.177-.38c0-1.84 3.145-1.877 7.602-1.738v1.002c0 1.128-1.171 2.168-4.075 2.168-2.725 0-3.527-.558-3.527-1.433z"
					/></svg
				>
			</a>
			<LangSwitch />
		</div>
	</div>

	<!-- <nav>
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L1,2 C1.5,3 1.5,3 2,3 L2,0 Z" />
		</svg>
		<ul>
			<li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
				<a href="/">Home</a>
			</li>
			<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
				<a href="/about">About</a>
			</li>
			<li aria-current={$page.url.pathname.startsWith('/sverdle') ? 'page' : undefined}>
				<a href="/sverdle">Sverdle</a>
			</li>
		</ul>
		<svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L0,3 C0.5,3 0.5,3 1,2 L2,0 Z" />
		</svg>
	</nav> -->
</header>

<style>
	header {
		background-color: var(--color-bg-0);
		padding: 16px 0;
	}
	.container {
		width: 1280px;
		margin: 0 auto;
	}
	.header-wrap {
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
</style>
