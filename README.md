# \<crob-property-selector\>

```<crob-property-selector>``` is a utility component that can used to extract values from a object. As a hybrid component, it is compatible with both Polymer 1.x and 2.x projects.

This component ensures that any changes applied to the object are propagated to any observers of the extracted value, and that any changes made to the extracted value are propagated back to the object.

## Usage

To use this component, simply set the **object** and **property** properties of the ```crob-property-selector``` and extract the result from the **value** property.

```html
<crob-property-selector
    object="[[object]]"
    property="[[property]]"
    value="{{value}}">
</crob-property-selector>
```

The **object** property defines the object or dictionary that holds the value you wish to extract.

The **property** property defines the name of the property that you wish to extract from the **object**.

The **value** property holds the value that the **object** has for the given **property**. In other words, if **object** is a dictionary and **property** is a key, then **value** is the same as **object[property]**.

You can also use this component to change values within the **object**, as any modifications made to the **value** property are reflected back into the object.