# shopifySnips

## Images
including images

	<img src="{{ 'image name with extension ie: name.png' | asset_img_url:'400x400' }}">
## Basic Schema
```
{% schema %}
  {
    "name": "Future ",
    "settings": [
  {
   "type": "text",
   "id": "this_section_id",
   "label": "SECTION TITLE"
  },
	],
	"presets": [
      {
        "name": "Future Products",
        "category": "Future Products"
      }
  ]
  }
{% endschema %}

```
## CSS Responsive
```
@mixin for-phone-only {
  @media (max-width: 599px) { @content; }
}
@mixin for-tablet-portrait-up {
  @media (min-width: 600px) { @content; }
}
@mixin for-tablet-landscape-up {
  @media (min-width: 900px) { @content; }
}
@mixin for-desktop-up {
  @media (min-width: 1200px) { @content; }
}
@mixin for-big-desktop-up {
  @media (min-width: 1800px) { @content; }
}

// usage
.my-box {
  padding: 10px;
  
  @include for-desktop-up {
    padding: 20px;
  }
}
```
## Blocks
```
"blocks": [
    {
      "type": "text",
      "name": "products",
      "settings": [
        {
          "type": "text",
          "id": "product_name",
          "label": "Product Name"
        }
      ]
    }
  ]
 ```
## can change what is shown on the product template based on if an item is available
``` 
  {% if product.available == true/false%}
  	show something here
  {% endif%}
  ```
