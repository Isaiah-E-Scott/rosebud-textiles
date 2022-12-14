# rosebud-textiles webpage

http://rosebudtextilesart.com

This is the source code of a client web page. 

## Responsive

It features responsive web desigm that adapts to many screen sizes automatically without the need to program multiple versions of the same page.

https://user-images.githubusercontent.com/14919064/206872277-86007145-94d4-46c8-af19-48d01d19e0d6.mp4

https://user-images.githubusercontent.com/14919064/206872590-9d28fc7f-3d8f-424d-ae28-80ac34fab032.mp4

## Interactive

It also features an interactive grid and tiles that can be hovered over to show more details or clicked on zoom in and show full resolution.

https://user-images.githubusercontent.com/14919064/206872798-3819a68e-c9b3-4b08-a4ad-ee8fce120667.mp4


**Here is the code to enable the hovering overlay:**
```
<div class="hover-bg"><a href="img/portfolio/BlossomingFlowers/Tropical_white_flowers_taupe_stock_preview.jpg" title="Flowers on Vines Red White Gold" data-lightbox-gallery="gallery1">
	<div class="hover-text">
		<h4>Tropical White Flowers Taupe</h4>
		<small>Blossoming Flowers</small>
	</div>
	<img src="img/portfolio/BlossomingFlowers/Tropical_white_flowers_taupe_stock_preview.jpg" class="img-responsive" alt="Flowers on Vines Red White Gold">
</a></div>
```

- class="hover-bg" - enables overlay over the object when a mouse hovers over it
- class="hover-text" - creates text in the overlay
- title - the text under the image in the zoomed view

## Grouping

Each tile can also be assigned a category so that it can be selected and sorted by its group.

https://user-images.githubusercontent.com/14919064/206873141-f35a011e-0bf7-45fc-8b2e-7efcc51cfdb2.mp4

**Here is the code to create the categiories:**

```
<div class="categories">
  <ul class="cat">
	<li>
	  <ol class="type">
		<li><a href="#" data-filter="*" class="active">All</a></li>
		<li><a href="#" data-filter=".stock">Stock Images</a></li>
		<li><a href="#" data-filter=".product">Product Sales</a></li>
		<li><a href="#" data-filter=".license">Licensing</a></li>
		<!--<li><a href="#" data-filter=".nothing">Nothing</a></li>-->
	  </ol>
	</li>
  </ul>
  <div class="clearfix"></div>
</div>
```
- data-filter is the variable that you assign to specify the category
    - data-filter="*" selects all of the items in the list regardless of the category
    - data-filter=".nothing" does not select any items in the list
        - this is currently unused so it has been commented out of the code
