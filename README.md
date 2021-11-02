# Youtube Videos Tracking

This code is useful when the native Youtube trigger doesn't work due to particular factors.
More information in the following article: https://www.analyticsmania.com/post/youtube-tracking-google-tag-manager-solved/


# What's included:

1) Custom Javascript - Is Youtube Present
2) cHTML - Youtube Listener
3) Custom - Youtube Interaction
4) asyncEvent - Youtube Is Present (da sostituire)
5) dlv - eventCategory
6) dlv - eventAction
7) dlv - eventLabel
8) GA - Event - Youtube Interaction

# How they work:

## 1) Custom Javascript - Is Youtube Present
A custom JS variable which return true  if there is at least one Youtube video on the page.

## 2) cHTML - Youtube Listener
This custom code contains a youtube listener which listen to changes of the youtube player every second. 
So even if the video is lazily loaded, after 1 second it will be tracked.
This code will push the "youtube" events to the dataLayer.

## 3) Custom - Youtube Interaction
A custom event used to trigger the Google Analytics event Tag.

## 4) ---

## 5)6)7) dlv
3 different dataLayer variables (dlv) used to track different events using a single Google Analytics tag.

## 8) GA - Event - Youtube Interaction



# How the final setup will work:




# Please Note
////
