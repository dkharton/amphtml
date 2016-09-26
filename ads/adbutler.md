<!---
Copyright 2015 The AMP HTML Authors. All Rights Reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

      http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS-IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

# AdButler

## Example

###Single Tag Example

```html
<amp-ad width=300 height=250
    type="adbutler"
    data-mid="123456"
    data-zone_id="123456"
    data-place="0">
</amp-ad>
```

###Two Tags, Same Zone
Note: Make sure that data-place is different each time the same zone tag is placed.
```html
<amp-ad width=300 height=250
    type="adbutler"
    data-mid="123456"
    data-zone_id="123456"
    data-place="0">
</amp-ad>
    
<amp-ad width=300 height=250
    type="adbutler"
    data-mid="123456"
    data-zone_id="123456"
    data-place="1">
</amp-ad>
```

###Two Tags, Different Zones
Note: Notice that data-place is 0 for both since they are different zones.
```html
<amp-ad width=300 height=250
    type="adbutler"
    data-mid="123456"
    data-zone_id="123456"
    data-place="0">
</amp-ad>
    
<amp-ad width=300 height=250
    type="adbutler"
    data-mid="123456"
    data-zone_id="654321"
    data-place="0">
</amp-ad>
```

###Single Tag With Keyword Targeting
```html
<amp-ad width=300 height=250
    type="adbutler"
    data-mid="123456"
    data-zone_id="123456"
    data-place="0"
    data-kw="green">
</amp-ad>
```
## Configuration

For semantics of configuration, please see [ad network documentation](https://www.adblade.com/doc/publisher-solutions).

Supported parameters:

Required:
- width
- height
- data-mid (AdButler account ID)
- data-zone_id

Optional:
- data-place
- data-kw
