1.Write a blog on Difference between HTTP1.1 vs HTTP2

HTTP/1.1 -

1.development of HTTP but we will focus mainly on HTTP/1.1 which was created in 1997

2.It works on the textual format

3.There is head of line blocking that blocks all the requests behind it until it doesn’t get its all resources.

4.There is head of line blocking that blocks all the requests behind it until it doesn’t get its all resources.

5.It compresses data by itself.

6.HTTP/1.1: For better understanding, let’s assume the situation when you make a request to the server for the geeksforgeeks.html page & server responds to you as a resource geeksforgeeks.html page. before sending the request and the response there is a TCP connection established between client & server. 
  again you make a request to the server for image img.jpg & the server gives a response as an image img.jpg. the connection was not lost here after the first request because we add a keep-alive header which is the part of the request so there is an open connection between the server & client. there is a persistent connection which means several requests & responses are merged in a single connection.

HTTP/2 -

1.development of HTTP new one is HTTP/2 which was created in 2015.

2.It works on the binary protocol.

3.It allows multiplexing so one TCP connection is required for multiple requests.

4.It uses PUSH frame by server that collects all multiple pages.

5.It uses HPACK for data compression.

6.HTTP/2: HTTP/2 was developed over the SPDY protocol. HTTP/2 works on the binary framing layer instead of textual that converts all the messages in binary format.
  it works on fully multiplexed that is one TCP connection is used for multiple requests. HTTP/2 uses HPACK which is used to split data from header. it compresses the header. The server sends all the other files like CSS & JS without the request of the client using the PUSH frame.

  

2.Write a blog about objects and its internal representation in Javascript
