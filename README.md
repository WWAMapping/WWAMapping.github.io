## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/WWAMapping/WWAMapping.github.io/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/WWAMapping/WWAMapping.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.

<DOCTYPE html>
<html>
  <head>
  <style>
    #map-canvas { width:500px; height:400px; }
    .layer-wizard-search-label { font-family: sans-serif };
  </style>
  <script type="text/javascript"
    src="http://maps.google.com/maps/api/js?sensor=false">
  </script>
  <script type="text/javascript">
    var map;
    var layer_0;
    var layer_1;
    var layer_2;
    function initialize() {
      map = new google.maps.Map(document.getElementById('map-canvas'), {
        center: new google.maps.LatLng(35.983794907103906, -94.25317571127823),
        zoom: 9,
        mapTypeId: google.maps.MapTypeId.ROADMAP
      });
      layer_0 = new google.maps.FusionTablesLayer({
        query: {
          select: "col2",
          from: "17t2FTlTMiPxmfnicNPg1m-ce-B4FolxQlZQCyAlP"
        },
        map: map,
        styleId: 2,
        templateId: 2
      });
      layer_1 = new google.maps.FusionTablesLayer({
        query: {
          select: "col2",
          from: "1k3xM2lbEJshAUtjL-HYx5t5KYq-09jCFFYyFLGMH"
        },
        map: map,
        styleId: 2,
        templateId: 2
      });
      layer_2 = new google.maps.FusionTablesLayer({
        query: {
          select: "col2",
          from: "10Qf3Vw9YCBHr0q7sF5ywrNBcg6Rd9GgbodNNRdTs"
        },
        map: map,
        styleId: 2,
        templateId: 2
      });
    }
    google.maps.event.addDomListener(window, 'load', initialize);
  </script>
  </head>
  <body>
    <div id="map-canvas"></div>
  </body>
</html>
