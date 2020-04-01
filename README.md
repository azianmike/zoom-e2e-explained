## Zoom E2E Encryption Explained Like You're 5

## Brief overview of encryption
Original message that we want to compress
```
Peanuts do not grow on trees. Cashews do grow on trees.
```
<br/>

Lossless -> Make the file smaller without any change in meaning or quality.

```
Peanuts don't grow on trees, but cashews do.
```
<br/>

Lossy -> Make file significantly smaller with small loss in meaning. 

```
Trees grow no peanuts, yes cashews
```

# Why can't we compress encrypted messages?
<br/>

Given our original message `Peanuts do not grow on trees. Cashews do grow on trees.`, if we encrypt it with a basic Caesar cipher, we get `Wlhubaz kv uva nyvd vu ayllz. Jhzoldz kv nyvd vu ayllz.`
<br/>

Let's assume we hand off `Wlhubaz kv uva nyvd vu ayllz. Jhzoldz kv nyvd vu ayllz.` to our friend, Alice, to help us compress the message. Let's also assume Alice does not know the original message nor how to decrypt the message we gave her.
<br/>

Alica can't compress the message and keep the same meaning because Alica never knew the original meaning to begin with.
<br/>

# Why does this matter for Zoom?

Zoom apparently says they are E2E encrypted and The Intercept claims Zoom is not truly E2E encrypted (https://theintercept.com/2020/03/31/zoom-meeting-encryption/).
<br/>
<br/>
It is well known that live streaming and video chats require compression and Zoom is no exception (https://blog.zoom.us/wordpress/2016/02/23/your-video-could-be-awesome/). To be clear, this compression is what makes Zoom so great; smooth video delivery for all network speeds.
<br/>
<br/>
For reasons I will not get into, this compression usually is not done on the client, mainly due to dynamic delivery of quality (ELI5 the quality of the video you receive can and will change). 
<br/>

TL;DR Either Zoom provides a great video conferencing experience that is not truly E2E encrypted or provides true E2E encryption with a bad video conference experience.




