# Svelte-Weather-Icons

SVG weather icons for Svelte. Svlete-Weather-Icons support major CSS framework. You can add additional CSS using the `class` props.


<p align="center">
<img width="450" src="https://raw.githubusercontent.com/shinokada/svelte-weather-icons/main/static/images/weather1.webp" />
<img width="450" src="https://raw.githubusercontent.com/shinokada/svelte-weather-icons/main/static/images/weather2.webp" />
</p>

## Original source

[erikflowers/weather-icons](https://github.com/erikflowers/weather-icons)

## List of icons

[Icon names](https://github.com/shinokada/svelte-weather-icons/blob/main/icon-list.md)

## Installation

```sh
npm i svelte-weather-icons
```

## REPL

- [Demo 1]()
- [Demo 2]()

## Usage

```js
<script>
  import { DayCloudy } from "svelte-weather-icons";
</script>
```

## Props

| Name      | Default   |
| --------- | --------- |
| size      | 30        |
| class     |           |
| ariaLabel | file name |

## Size

Use the `size` prop to change the size of icons.

```html
<DayCloudy size="30" />
<DayCloudy size="40" />
<DayCloudy size="50" />
```

## CSS HEX Colors

Use the `color` prop to change colors with HEX color code.

```html
<DayCloudy color="#ff0000" />
<DayCloudy color="#00ffd8" />
```

## CSS framework support

Use the `class` prop to change colors and add additional css.

For example, Tailwind CSS:

```html
<DayCloudy class="text-pink-700 mr-4" />
```

If you use the dark mode on your website with Tailwind CSS, add your dark mode class to the `class` prop.

Let's use `dark` for the dark mode class as an example.

```html
<DayCloudy class="text-pink-700 dark:text-blue-300" />
```

Bootstrap example:

```html
<DayCloudy class="position-absolute top-0 px-1" />
```


## aria-label

All icons have aria-label. For example `DayCloudy` has `aria-label="day cloudy"`. 
Use `ariaLabel` prop to modify the `aria-label` value. 

```html
<DayCloudy ariaLabel="day cloudy icon" class="text-red-500">
```

## Passing down other attributes

You can pass other attibutes as well.

```html
<DayCloudy tabindex="0">
```

## Import all

Use `import * as Icon from 'svelte-weather-icons`.

```html
<script>
  import * as Icon from "svelte-weather-icons";
</script>

<Icon.DayCloudy size="30" class="text-red-500" />
<Icon.DirectionRight size="40" class="text-blue-700" />
<Icon.Hail size="50" class="text-green-700" />
<Icon.MoonAltWaningGibbous2 size="60" class="text-purple-500" />
<Icon.NightAltSleet size="100" class="text-purple-500" tabindex="0" />
```


## Other icons

- [Svelte-Icon-Sets](https://svelte-svg-icons.vercel.app/)