# Tealium Collect template for Google Tag Manager

## Overview

This is the Google Tag Manager template for the Tealium Collect tag.

The Tealium Collect tag template allows you to enable and configure data collection for Tealium's Customer Data Hub (CDH) on your website using Google Tag Manager.

For more information on Tealium's CDH, please visit [Tealium's Learning Community](https://community.tealiumiq.com/t5/Customer-Data-Hub/Introduction-to-Customer-Data-Hub/ta-p/17571)

## Quickstart Configuration

1. Search the Google Tag Manager Community Template Gallery for "Tealium Collect"
2. Add this template
3. Create a new tag from this template
4. Enter the Tealium Account, Profile, and Data Source Key obtained from Tealium's CDH
5. Subscribe your tag to the events you wish to track.  Use "All Pages" trigger to get started tracking page views.  All Events are supported.


## Advanced Configuration

Tealium recommends triggering this tag for All Events execepting the gtm.dom and gtm.load events.

Tealium Collect tag template also allows for advanced configuration settings:

1. First-party data collection

If your network team has worked with Tealium to configure a first-party data collection endpoint, then you should use the full endpoint URL here (not just the domain).  Consult your Account Manager or Implementation Engineer for more information.

2. Adding Custom Attributes

Use the mapping table to either add or replace an item to your data layer when the tag is triggered.  This might be something you want to add to every event in addition to the values found in the dataLayer.push calls.

For example, if you do not wish to use the default 'event' value for 'tealium\_event' then add an entry to override 'tealium\_event'.  If you want to add a new attribute 'blog\_topic' then map this to either a static value or any dynamic Variable.

3. Custom Data Object

By default, the Tealium Collect tag template uses the global 'dataLayer' array/object as the data layer.  However, if you have changed your global object name or want to enhance the existing dataLayer object with additional data, you can create a 'Custom JavaScript' Variable function to build and return a different object for the data layer.

4. Merge Data from Previous Events

Check this box to add all data attributes from previous dataLayer.push calls.  If this box is not checked, only previous attributes are merged in for data objects that did not have an 'event' attribute.

## Additional Resources

**[Documentation](https://docs.tealium.com/platforms/google-tag-manager/install/)**

## Copyright and license

Copyright 2020 Tealium Inc. All rights reserved.

Licensed under the **[Apache License, Version 2.0][license]** (the "License");
you may not use this software except in compliance with the License.

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

