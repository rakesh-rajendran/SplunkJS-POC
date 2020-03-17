# SplunkJS-POC
SplunkJS POC

* Issues with Custom Visualization for Splunk Web & Converted Dashbord HTML.docx - Explains the issues.
* splunk-js.zip - This contains the SplunkJS libraries and the HTMLs required for troubleshooting the issue.
* viz_tutorial_app.zip - This contains the Custom Vizualization created.

:speech_balloon:
- [nginx](http://nginx.org/en/download.html) server is used as Proxy (configured to listen in port 9000). This was required while connecting from external web apps since no_proxy configurations was failing with **err_cert_authority_invalid** error.
- Addtionally, Use a *'Security Disabled'* browser. [Disable CORS] (https://alfilatov.com/posts/run-chrome-without-cors/)

Example - "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --user-data-dir="C:\Users\rakesh.rajendran\AppData\Local\Google\Chrome DEV" --disable-web-security


## viz_tutorial_app.zip 

* Extract this zip file under **%SPLUNK_HOME/etc/apps** . Refer [Issues with Custom Visualization for Splunk Web & Converted Dashbord HTML.docx](https://github.com/rakesh-rajendran/SplunkJS-POC/blob/master/Issues%20with%20Custom%20Visualization%20for%20Splunk%20Web%20%26%20Converted%20Dashbord%20HTML.docx)

## splunk-js.zip
- Extract this zip inside a folder.
  - A directory **static** with all SplunkJS libraries should be extracted
  - **login_form.html** - To enable logging to Splunk and retrive a Session key
  - **customviz1.html** - This holds the HTML to load the custom vizualization using SplunkJS
  - **splunk_custom_dashboard_manual_HTML** - This holds the HTML of the Splunk converted HTML

