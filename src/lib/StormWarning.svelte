<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let ariaLabel = 'storm warning';
</script>

<svg
  version="1.1"
  id="Layer_1"
  xmlns="http://www.w3.org/2000/svg"
  xmlns:xlink="http://www.w3.org/1999/xlink"
  x="0px"
  y="0px"
  width={size}
  height={size}
  {...$$restProps}
  {role}
  aria-label={ariaLabel}
  fill={color}
  on:click
  on:keydown
  on:keyup
  on:focus
  on:blur
  on:mouseenter
  on:mouseleave
  on:mouseover
  on:mouseout
  viewBox="0 0 30 30"
  style="enable-background:new 0 0 30 30;"
  xml:space="preserve"
>
  <path
    d="M9.76,24.6V7.45h1.13V24.6H9.76z M11.7,14.05v-6.6h8.55v6.6H11.7z M14.06,12.05h3.81v-2.5h-3.81V12.05z"
  />
</svg>

<!--
@component
[Go to docs](https://svelte-weather-icons.vercel.app/)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
@prop export let ariaLabel = 'storm warning';
-->
