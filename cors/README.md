# CORS - Enable Alfresco for CORS
I did a Lightning Talk[^[https://www.slideshare.net/jottley/cors-enable-alfresco-for-cors](https://www.slideshare.net/jottley/cors-enable-alfresco-for-cors)] at Alfresco Summit in 2013 (Barcelona[^[https://summit.alfresco.com/barcelona/sessions](https://www.slideshare.net/jottley/cors-enable-alfresco-for-cors)]/Boston[^[https://summit.alfresco.com/boston/sessions](https://www.slideshare.net/jottley/cors-enable-alfresco-for-cors)]) on enabling Alfresco to support CORS[^[https://en.wikipedia.org/wiki/Cross-origin_resource_sharing](https://www.slideshare.net/jottley/cors-enable-alfresco-for-cors)]. We had implemented this for the initial Salesforce Connector (v1) and there was interest in making the same thing possible for the on-premise platform. 

In Alfresco 5.0, we introduced the config and library[^[http://software.dzhuvinov.com/cors-filter.html](https://www.slideshare.net/jottley/cors-enable-alfresco-for-cors)] as part of the core platform.  It was disabled by default but it was now possible to build Web Applications that could make cross-domain calls without needing to inject additional changes.
  
The talk covers the basics of what CORS is and how to enable it  in Alfresco (pre 5.0). The concepts still apply to current versions of Alfresco. The sample code from the demo is in this project[^[https://github.com/jottley/memory/tree/master/cors](https://www.slideshare.net/jottley/cors-enable-alfresco-for-cors)]. The demo video is available on youtube[^[https://www.youtube.com/watch?v=il1ZlEBqvLU](https://www.slideshare.net/jottley/cors-enable-alfresco-for-cors)].

Gethin James[^[https://twitter.com/covolution](https://www.slideshare.net/jottley/cors-enable-alfresco-for-cors)] has simplified enabling CORS by providing a simple module[^[https://github.com/covolution/enablecors](https://www.slideshare.net/jottley/cors-enable-alfresco-for-cors)] that can be added to you Alfresco instance. It can be added your projects using maven:

`<dependency>
  <groupId>org.alfresco</groupId>
  <artifactId>enablecors</artifactId>
  <version>1.0</version>
</dependency>`
