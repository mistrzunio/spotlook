# spotlook
Spotlight Metadata Query to be used with Outlook for Mac to filter robot, automated e-mails, whatever custom Query you wish to add

## How to use it
Works with Outlook for Mac, tested with v16 on Sierra

#### 1. In the upper-right corner of the Outlook window, click in the search box.

The Search tab appears.

#### 2. Click one of criteria buttons, i.e.: Subject

The Criteria Bar appears below ribbon, i.e.: _Subject > Contains > search field_

#### 3. Change Criteria from *Subject* to *Raw Query*

#### 4. Paste follwing sample Query and see what happens:

```
kMDItemTitle == "Accepted:*" ||
kMDItemTitle == "Canceled:*" ||
kMDItemTitle == "*OOO" || 
kMDItemTitle == "OOO*" || 
kMDItemTitle == "*OoO" || 
kMDItemTitle == "*WFH" ||
kMDItemTitle == "WFH*" ||
kMDItemTitle == "Missed conversation with*" ||
kMDItemTitle == "[Slack] Notifications*" || 
kMDItemTitle == "*updates for the week of*" || 
kMDItemTitle == "*Newsletter" || 
kMDItemTitle == "Action Required*" || 
kMDItemTitle == "ACTION REQUIRED*" || 
kMDItemTitle == "NO ACTION REQUIRED*" || 
kMDItemTitle == "*Submitted" || 
kMDItemTitle  == "*has accepted the invitation*folder on Box" || 
kMDItemAuthors  == "Box Updates*" || 
kMDItemAuthors  == "Communications Team*" || 
kMDItemAuthors  == "HR update*" || 
kMDItemAuthors  == "*on Yammer*"
```

#### 5. _`[optional]`_ You can add additional criteria on this point

Just clik small **+** icon, then select criteria, conditions, etc i.e.: *Follow Up Flag > Not Flagged*

#### 5. Click *Save Search* to create Smart folder


### References:
Spotlight Metadata Attributes <https://developer.apple.com/library/archive/documentation/CoreServices/Reference/MetadataAttributesRef/Reference/CommonAttrs.html#//apple_ref/doc/uid/TP40001694-SW1>

File Metadata Query Expression Syntax <https://developer.apple.com/library/archive/documentation/Carbon/Conceptual/SpotlightQuery/Concepts/QueryFormat.html>
