SCORM Manifest Template for ingest into compliant LMS.

Assumes SCORM 1.2 calls. Opens an iframe and uses postMessage to send info back and forth.

Model of data object to send out to parent receiver:

{

	type: 'scorm',
	method: 'get' or 'set',
	model: name of data model to change (ex: 'cmi.core.score.raw'),
	value: if setting data this is the value you want to set (ex: 100)
}

The receiver will pass information back to the iframe eventListener. Look at the index.html to see how this is performed.

Edit the index.html file content_url variable to point to the right webpage.