# SmileEzEESectionFormFieldBundle

[![SensioLabsInsight](https://insight.sensiolabs.com/projects/b3954da8-43b5-4394-a233-28113d57676c/mini.png)](https://insight.sensiolabs.com/projects/b3954da8-43b5-4394-a233-28113d57676c)

Add new eZStudio Form Field named *Section* to organize Form Fields.

This new Field is not really a Form Field, just a Form section delimiter.

## Installation

### Get the bundle using composer

Add SmileEzEESectionFormFieldBundle by running this command from the terminal at the root of
your eZStudio project:

```bash
composer require smile/ezee-sectionformfield-bundle
```


### Enable the bundle

To start using the bundle, register the bundle in your application's kernel class:

```php
// ezpublish/EzPublishKernel.php
public function registerBundles()
{
    $bundles = array(
        // ...
        new Smile\EzEESectionFormFieldBundle\SmileEzEESectionFormFieldBundle(),
        // ...
    );
}
```

### Add  assetic

 ```
 {% stylesheets filter='cssrewrite'
     ...
     'bundles/smileezeesectionformfield/css/smileform_section.css'
 %}
     <link rel="stylesheet" type="text/css" href="{{ asset_url }}">
 {% endstylesheets %}
```
