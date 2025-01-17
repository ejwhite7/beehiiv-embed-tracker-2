# beehiiv Embed Tracker v2
## Why?
I found when auditing a client account that we don't nearly enough to capture and parse utm and referral info that can be used to give users qualitative data around growth. 

For example, any one coming from an embed without UTM parameters is marked as embed: direct/(none) where we could be looking at the referrer and parameters to understand traffic.

With this script, is there are no utm_source or utm_medium params and the referrer is google.com then the script understands that this is organic referral traffic and ads the tracking data as embed: google / organic. 

Similarly, if a user were to come from a Facebook ad, but not an utm_params manually set, we'd see the fbclid and parse it as "embed: facebook / paid".
