---
title: Add Barcodes to a Report
author: Anna Gubareva
---
# Add Barcodes to a Report

## Overview

To insert a barcode into a report, drag the **Barcode** item from the [Toolbox](../../report-designer-tools/toolbox.md) onto the report's area.

![](../../../../../images/eurd-win-add-bar-code-to-report.png)

After creating the barcode, select the barcode type (symbology) in the **Barcode Tools** [toolbar](../../report-designer-tools/toolbar.md) tab's **Symbology** gallery.
	
![](../../../../../images/eurd-win-bar-code-symbology.png)
	
After specifying the symbology, you can customize the type-specific options of the barcode, which are listed in the [Property Grid](../../report-designer-tools/ui-panels/property-grid-tabbed-view.md) under the **Symbology** property.
	
![](../../../../../images/eurd-win-bar-code-symbology-property.png)

## Main Options

You can use the **Binary Data** property to supply the data that a barcode should encode.

To specify the bar width (a barcode's resolution), use the following options:
	
* Automatically calculate the bar width according to a barcode's dimensions by enabling the **Auto Module** option;
* Provide a fixed bar width value using the **Module** property.

The following are some additional barcode options:
	
* Use the barcode's **Text** property to provide accompanying text. The **Show Text** property allows you to show or hide this text.

* Use the **Orientation** property to rotate a barcode.

* Use the **Padding** property to specify the indent between bars and the barcode's inner boundaries.

## Bind to Data

You can [bind](../bind-controls-to-data.md) the bar code's **Text** property to a data field obtained from a report's data source. Click the control's smart tag, expand the **Expression** drop-down list and select the data field.

![](../../../../../images/eurd-win-bar-code-bind-to-data.png)

You can also click the **Expression** option's ellipsis button to invoke the **Expression Editor**. This editor allows you to construct a complex binding expression with two or more data fields.

## Common Errors
The following section explains how to work around the most frequently encountered errors related to the incorrect use of barcodes.

* The following error message is shown in place of the barcode if the control's dimensions are too small to fit the barcode with its specified resolution.
	
	![](../../../../../images/eurd-win-bar-code-small-boundaries-error.png)
	
	To get rid of this error, enable the **Auto Module** property and/or increase the barcode's dimensions.

* The following error message appears when the data supplied to a barcode contains characters that are not supported by this barcode type.
	
	![](../../../../../images/eurd-win-bar-code-invalid-characters-error.png)
	
	To avoid this error, supply data that applies to a particular barcode specification.
