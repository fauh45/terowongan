# Terowongan Protocol

The focus of the implementation would be on making HTTP CONNECT method works. The method itself is a standard part of HTTP/1.1 standard method used to establish a tunnel connection with a proxy (see: [rfc2616](https://datatracker.ietf.org/doc/html/rfc2616#section-9.9)).

## HTTP Tunnel

HTTP tunnel is first defined in rfc in progress referenced by [rfc2616](https://datatracker.ietf.org/doc/html/rfc2616#section-9.9) titled "Tunneling TCP based protocols through Web proxy servers" (see the [draft](https://www.ietf.org/archive/id/draft-luotonen-web-proxy-tunneling-01.txt)) but was never made part of IETF Standard. But the method was widely implemented by HTTP proxies. So for terowongan we're going to be referencing that work for the implementation, as it is widely used anyway. And also it was referenced on a [rfc2817](https://datatracker.ietf.org/doc/html/rfc2817).

The draft specifies that the CONNECT method follows the same HTTP/1.x protocol. All the initial setup is done like a normal HTTP call would. Below, I've made a high level UML Sequence diagram to show simply how it works (without auth, ideal condition).

![High Level Sequence Diagram of HTTP Tunneling](./images/HTTP%20Proxy%20High%20Level%20Sequence%20Diagram.png)
