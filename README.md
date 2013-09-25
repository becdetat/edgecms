edgecms
=======

A minimal, drop-in, highly component based, and did I mention minimal, content management system

In fact it is so minimal it consists of this readme. Written on an iPod because I can't sleep. 

## design goals
- core system requires a storage mechanism, a renderer, an editor, and a security facility. In fact all it will provide is a mapping between the editor, the renderer, and the storage mechanism. It will look after the logic of finding content for a given content query.
- output will be markdown by default but it is really agnostic of the content markup
- provide an in memory reference data store
- provide a dropin wysiwyg editor
- data store needs to store and retrieve text content and binary content (images and attachments)
- should not rely on asp.net
- core should not try to manage images or attachments per content page
- no need for templates, that should be the concern of the consumer
- core should work on monotouch
- monotouch (iOS) compatible proxy 'server' component
	- imagine being able to pull back an entire site for local storage, then each request goes through the proxy, boosting performance and adding offline capability


