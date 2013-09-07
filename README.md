# Vapors
An unobtrusive, markup agnostic, responsive grid utility for SASS projects.

## Installation

### Bower:
```
bower install vapors
``` 
## Disclaimer 
Vapors depends on `inline-block` and expects the user to be aware of the whitespace quirks in their markup.

### Wrong
```
<div class='wrap'>
	<div class="col">
		
	</div>
	<div class="col">

	</div>
</div>
```
### Right
```
<div class='wrap'>
	<div class="col">
		
	</div><div class="col">

	</div>
</div>
```

## Usage

### In Markup
```
  <div class="selector col">
  </div>
```

### In SCSS
```
 .selector {
  @include set-vapors(
      <breakpoint-name> <col-span>, 
      <breakpoint-name> <col-span>
  );
}
``` 