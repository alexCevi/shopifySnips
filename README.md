# shopifySnips

## Images
including images

	<img src="{{ 'image name with extension ie: name.png' | asset_img_url:'400x400' }}">
## Basic Schema
```
{% schema %}
  {
    "name": "Future Products",
    "settings": [
  {
   "type": "text",
   "id": "about_text",
   "label": "About soNeat"
  },
	],
	"presets": [
      {
        "name": "Future Products",
        "category": "Future Products"
      }
  ],
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
  }
{% endschema %}

```
