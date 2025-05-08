# Hugx

Hugo shortcode to create an image gallery. This is intended to be used
in a Hugo project along with an existing theme.

## Installation

Import the module from GitHub repository.

```yaml
# hugo.yaml
module:
  imports:
    - path: github.com/tnlx/hugx-gallery
```

## Usage

### Styles

```css
/* assets/scss/main.scss */
@use 'hugx/gallery';
```

### Data

```yaml
# data/jonas.yaml
---
- imgSrc: /picture.jpg
  title: hugx-1
  subtitle: A brief description of this image
  url: "#"
- imgSrc: /picture1.jpg
  title: hugx-2
  subtitle:
  url: "#"
```

### Content

```
hugx/gallery src="jonas.yaml"
```
