OAuth bounce pages for deux par deux internal CLIs. Static only.
Each page forwards the browser to http://localhost:<port>/callback with the same query string,
where the local CLI (dpd-tools/tools/*_q.py auth) is listening.
Nothing is stored or logged here.
