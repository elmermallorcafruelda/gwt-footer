# Goverment Website Template (GWT) footer script generator
**Authored by: Voltz Jeturian voltz.jeturian@icto.dost.gov.ph**

#### v0.2-beta

The gwt-footer is a footer script generator for GWT template. The main purpose of having a footer generator is to provide a uniform feel and enforce the guideline of the standard footer. The footer generator automatically retrieves the updated version of html codes of the footer template to ensure that the contents and the links are up to date.

##Note
This version is **BETA** only and experimental and shoud be tested on a development server before releasing for the production server. For support, comments, suggestions, and if you found any bugs, please email us at **gwtsupport@i.gov.ph**

### How to add footer generator
To add the footer generator on your template, simply add this syntax to your template.

```
<div id="gwt-standard-footer">
</div>
<script>
    (function(d, s, id) {
      var js, gjs = d.getElementById('gwt-standard-footer');

      js = d.createElement(s); js.id = id;
      js.src = "http://gwt-footer.googlecode.com/git/footer.js";
      gjs.parentNode.insertBefore(js, gjs);

    }(document, 'script', 'gwt-footer-jsdk'));
</script>
```
**Note** that gwt-standard-footer id is where the standard footer will embed, so rename your footer container id to "gwt-standard-footer".

###### CHANGE LOGS
**06-25-2014**
- created GWT footer script generator

**07-01-2014**
- added automated script that generates template from source code
- added embed script sample to index.html for sample

**07-29-2014**
- added autoresizer script
