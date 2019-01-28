# Service Requests Without Response

Just a small repository to keep information about project I worked on during
Google Summer of Code 2016 with [Open Source Robotics Foundation](http://www.osrfoundation.org/).

## Project Info

Ignition transport is a component in the [ignition framework](http://ignitionrobotics.org),
a set of libraries designed to rapidly develop robot applications. The
[Ignition Transport](http://ignitionrobotics.org/libraries/transport) library
combines [ZeroMQ](http://zeromq.org/) with [Protobufs](https://developers.google.com/protocol-buffers/)
to create a fast and efficient message passing system. Asynchronous message publication and
subscription is provided along with service calls and discovery.

Not all the service requests in Ignition Transport library require a response.
So, we removed the service request handler after sending the request, instead of
waiting for the response for such requests which do not require a response back.

With this average time taken for a service request has been reduced.

[GSoC Archive](https://summerofcode.withgoogle.com/archive/2016/projects/6433512848621568/)

[Commits](https://bitbucket.org/ignitionrobotics/ign-transport/commits/all?search=user(Amitoj))
