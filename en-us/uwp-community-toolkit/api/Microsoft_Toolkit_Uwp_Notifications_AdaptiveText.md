
# AdaptiveText class

An adaptive text element.

## Members

The **AdaptiveText** class has this types of members

* [methods](#methods)

* [properties](#properties)

### methods

#### ToString()

Returns the value of the Text property.

##### parameters



| name | description | type |
### properties

#### Text

The text to display.

#### Language

The target locale of the XML payload, specified as a BCP-47 language tags such as "en-US" or "fr-FR". The locale specified here overrides any other specified locale, such as that in binding or visual. If this value is a literal string, this attribute defaults to the user's UI language. If this value is a string reference, this attribute defaults to the locale chosen by Windows Runtime in resolving the string.

#### HintStyle

The style controls the text's font size, weight, and opacity. Note that for Toast, the style will only take effect if the text is inside an [AdaptiveSubgroup](Microsoft_Toolkit_Uwp_Notifications_AdaptiveSubgroup.md).

#### HintWrap

Set this to true to enable text wrapping. For Tiles, this is false by default. For Toasts, this is true on top-level text elements, and false inside an [AdaptiveSubgroup](Microsoft_Toolkit_Uwp_Notifications_AdaptiveSubgroup.md). Note that for Toast, setting wrap will only take effect if the text is inside an [AdaptiveSubgroup](Microsoft_Toolkit_Uwp_Notifications_AdaptiveSubgroup.md) (you can use HintMaxLines = 1 to prevent top-level text elements from wrapping).

#### HintMaxLines

The maximum number of lines the text element is allowed to display. For Tiles, this is infinity by default. For Toasts, top-level text elements will have varying max line amounts (and in the Anniversary Update you can change the max lines). Text on a Toast inside an [AdaptiveSubgroup](Microsoft_Toolkit_Uwp_Notifications_AdaptiveSubgroup.md) will behave identically to Tiles (default to infinity).

#### HintMinLines

The minimum number of lines the text element must display. Note that for Toast, this property will only take effect if the text is inside an [AdaptiveSubgroup](Microsoft_Toolkit_Uwp_Notifications_AdaptiveSubgroup.md).

#### HintAlign

The horizontal alignment of the text. Note that for Toast, this property will only take effect if the text is inside an [AdaptiveSubgroup](Microsoft_Toolkit_Uwp_Notifications_AdaptiveSubgroup.md).