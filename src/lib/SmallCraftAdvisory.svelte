<script>
  export let size = '30';
  export let role = 'img';
  export let color = 'currentColor';
  export let ariaLabel = 'small craft advisory';
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
  <path d="M9.81,24.6V7.45h1.03V24.6H9.81z M11.54,14.86V7.45l8.65,3.69L11.54,14.86z" />
</svg>

<!--
@component
[Go to docs](https://svelte-weather-icons.vercel.app/)
## Props
@prop export let size = '30';
@prop export let role = 'img';
@prop export let color = 'currentColor';
@prop export let ariaLabel = 'small craft advisory';
-->
