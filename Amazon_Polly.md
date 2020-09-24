## Amazon Polly for Text to Speech

Support many lannguages
Support many voices
can customize with lexicon
Works with Speech Synthesis Markup Language (SSML)


Polly Use Case : Talking IoT

IoT Sensors --> AWS IoT + Lambda --> IoT Loudspeaker --> Amazon Polly

_AWS IoT + Lambda_ - AWS IoT receives signal and calls Lambda function to get a pre-signed URL to Polly with test of notification, **"Sean's room is getting Cold."**

IoT Loudspeaker --> This receives pre-signed URL and uses it to request speech audio from Polly.

Amazon Polly --> Polly receives text and streams speech audio back to be played on the loudspeaker.

