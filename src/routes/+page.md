# Svelte Weather

<div class="flex gap-2 my-8">
<a href="https://github.com/sponsors/shinokada" target="_blank"><img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86" alt="sponsor" height="25" style="height: 25px !important;"></a>
<a href="https://www.npmjs.com/package/svelte-weather" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/v/svelte-weather" alt="npm" height="25" style="height: 25px !important;"></a>
<a href="https://twitter.com/shinokada" rel="nofollow" target="_blank"><img src="https://img.shields.io/badge/created%20by-@shinokada-4BBAAB.svg" alt="Created by Shin Okada" height="25" style="height: 25px !important;"></a>
<a href="https://opensource.org/licenses/MIT" rel="nofollow" target="_blank"><img src="https://img.shields.io/github/license/shinokada/svelte-weather" alt="License" height="25" style="height: 25px !important;"></a>
<a href="https://www.npmjs.com/package/svelte-weather" rel="nofollow" target="_blank"><img src="https://img.shields.io/npm/dw/svelte-weather.svg" alt="npm" height="25" style="height: 25px !important;"></a>
</div>

210+ SVG weather icons for Svelte.

Thank you for considering my open-source package. If you use it in a commercial project, please support me by sponsoring me on GitHub: https://github.com/sponsors/shinokada. Your support helps me maintain and improve this package for the benefit of the community.


## Repo

[GitHub Repo](https://github.com/shinokada/svetle-weather)

## Original source

[erikflowers/weather-icons GitHub Repo](https://github.com/erikflowers/weather-icons)

## License

[Svelte-Weather License](https://github.com/shinokada/svetle-weather/blob/main/LICENSE)

[erikflowers/weather-icons LICENSE](https://github.com/erikflowers/weather-icons#licensing)


## Installation

```sh
pnpm i svelte-weather
```

## Usage

```js
<script>import {DayCloudy} from "svelte-weather";</script>
```

## Faster compiling

If you need only a few icons from this library in your Svelte app, import them directly. This can optimize compilation speed and improve performance by reducing the amount of code processed during compilation.

```html
<script>
  import DayCloudy from 'svelte-weather/DayCloudy.svelte';
</script>

<DayCloudy />
```

If you are a TypeScript user, install **typescript version 5.0.0 or above**.

```sh
pnpm i -D typescript@beta
```

To avoid any complaints from the editor, add `node16` or `nodenext` to `moduleResolution` in your tsconfig.json file.

```json
{
  //...
  "compilerOptions": {
    // ...
    "moduleResolution": "nodenext"
  }
}
```

## Props

- size = '30';
- role = 'img';
- color = 'currentColor';
- ariaLabel = 'icon file name';

## IDE support

If you are using an LSP-compatible editor, such as VSCode, Atom, Sublime Text, or Neovim, hovering over a component name will display a documentation link, features, props, events, and an example.

## Size

Use the `size` prop to change the size of icons.

```html
<DayCloudy size="30" />
<DayCloudy size="40" />
<DayCloudy size="50" />
```

If you are using Tailwind CSS, you can add a custom size using Tailwind CSS by including the desired classes in the class prop. For example:

```html
<DayCloudy class="shrink-0 h-20 w-20" />
```

## CSS HEX Colors

Use the `color` prop to change colors with HEX color code.

```html
<DayCloudy color="#ff0000" /> <DayCloudy color="#00ffd8" />
```

## CSS framework support

You can apply CSS framework color and other attributes directly to the icon component or its parent tag using the `class` prop.

For example, Tailwind CSS:

```html
<DayCloudy class="text-pink-700 mr-4" />
```

Bootstrap example:

```html
<DayCloudy class="position-absolute top-0 px-1" />
```

## Dark mode

If you use the dark mode on your website with Tailwind CSS, add your dark mode class to the `class` prop.

Let's use `dark` for the dark mode class as an example.

```html
<DayCloudy class="text-pink-700 dark:text-blue-300" />
```

## aria-label

All icons have aria-label. For example `DayCloudy` has `aria-label="day cloudy"`.
Use `ariaLabel` prop to modify the `aria-label` value.

```html
<DayCloudy ariaLabel="day cloudy icon" class="text-red-500" />
```

## Unfocusable icon

If you want to make an icon unfocusable, add `tabindex="-1"`.

```html
<DayCloudy tabindex="-1" />
```

## Events

All icons have the following events:

- on:click
- on:keydown
- on:keyup
- on:focus
- on:blur
- on:mouseenter
- on:mouseleave
- on:mouseover
- on:mouseout

## Passing down other attributes

You can pass other attibutes as well.

```html
<DayCloudy tabindex="0" />
```

## Using svelte:component

```html
<script>
  import { DayCloudy } from 'svelte-weather';
</script>

<svelte:component this="{DayCloudy}" />
```

## Using onMount

```html
<script>
  import { DayCloudy } from 'svelte-weather';
  import { onMount } from 'svelte';
  const props = {
    size: '50',
    color: '#ff0000'
  };
  onMount(() => {
    const icon = new DayCloudy({ target: document.body, props });
  });
</script>
```

## Import all

Use `import * as Icon from 'svelte-weather`.

```html
<script>
  import * as Icon from 'svelte-weather';
</script>

<Icon.DayCloudy size="30" class="text-red-500" />
<Icon.DirectionRight size="40" class="text-blue-700" />
<Icon.Hail size="50" class="text-green-700" />
<Icon.MoonAltWaningGibbous2 size="60" class="text-purple-500" />
<Icon.NightAltSleet size="100" class="text-purple-500" tabindex="0" />
```

## Other icons

[Svelte-Icon-Sets](https://svelte-svg-icons.vercel.app/)
