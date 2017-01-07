# Magento2 Module Select2 Ui Component

Select2 UI Component for Magento 2


## Installation

1. `composer require weprovide/magento2-module-select2-uicomponent`
2. `bin/magento setup:upgrade`

## Usage

It can be used in any UI Component configuration file.

Example:

`VENDOR/MODULE/view/adminhtml/ui_component/cms_page_form.xml`

```xml
<?xml version="1.0" encoding="UTF-8"?>
<form xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="urn:magento:module:Magento_Ui:etc/ui_configuration.xsd">
    <fieldset name="FIELDSET_NAME">
        <field name="CUSTOM_FIELD">
            <argument name="data" xsi:type="array">
                <item name="options" xsi:type="object">VENDOR\MODULE\Model\Config\Source\CUSTOMSOURCE</item>
                <item name="config" xsi:type="array">
                    <item name="dataType" xsi:type="string">text</item>
                    <item name="label" xsi:type="string" translate="true">CUSTOM FIELD</item>
                    <item name="formElement" xsi:type="string">select</item>
                    <item name="source" xsi:type="string">page</item>
                    <item name="dataScope" xsi:type="string">CUSTOM_FIELD</item>
                    <item name="elementTmpl" xsi:type="string">WeProvide_Select2UiComponent/form/element/select2</item>
                </item>
            </argument>
        </field>
    </fieldset>
</form>
```
