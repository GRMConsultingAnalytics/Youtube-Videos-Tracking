# Youtube Videos Tracking

This code is useful when the native Youtube trigger doesn't work due to particular factors.
More information in the following article: https://www.analyticsmania.com/post/youtube-tracking-google-tag-manager-solved/


# What's included:

1) Custom Javascript - Is Youtube Present
2) cHTML - Youtube Listener
3) Custom - Youtube Interaction
4) DOM - Youtube Is Present
5) dlv - eventCategory
6) dlv - eventAction
7) dlv - eventLabel
8) GA - Event - Youtube Interaction

# How they work:

### 1) Custom Javascript - Is Youtube Present
A custom JS variable which return true  if there is at least one Youtube video on the page.

### 2) cHTML - Youtube Listener
This custom code contains a youtube listener which listen to changes of the Youtube player every second. 
So even if the video is lazily loaded, after 1 second it will be tracked.
This code will push the "youtube" events to the dataLayer.

### 3) Custom - Youtube Interaction
Custom event used to trigger the Google Analytics event Tag.

### 4) DOM - Youtube Is Present
Trigger used to fire the GA event tag.
The trigger type is "Page View - DOM Ready" and it fires only when the "Custom Javascript - Is Youtube Present" variable equals true

### 5) dlv - eventCategory
dataLayer variable used to track the event category in "GA - Event - Youtube Interaction" tag.

### 6) dlv - eventAction
dataLayer variable used to track the event action in "GA - Event - Youtube Interaction" tag.

### 7) dlv - eventLabel
dataLayer variable used to track the event label in "GA - Event - Youtube Interaction" tag.

### 8) GA - Event - Youtube Interaction
Google Analytics event tag used to track the Youtube video interaction.


# How the final setup will work:

Every time the page is loaded the "Custom Javascript - Is Youtube Present" checkS if there is at least one Youtube video on the page.
If a video is present the "cHTML - Youtube Listener" will fire start listening to changes of the Youtube player pushing the events related to play and view percentage
into the dataLayer.


# Please Note
This script represents a plan B and may cause the video to flicker. It is suggested to test the YouTube Video trigger first.
You can find the trigger documentation following this link: https://support.google.com/tagmanager/answer/7679325?hl=en




