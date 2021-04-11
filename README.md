# wrk - a HTTP benchmarking tool

  Congrats on great woke, fella homo ape. <fold these feelz> I just wanna 2 say hi 2 wierd drugs... dev oops, thats not what i wanna soy<...> thq & congrats on universes branch.
  Ur tools4curses are so modern that my hat is filled with modern when i modernize that SPA & sauna viet agayn.

  wrk is a modern HTTP benchmarking tool capable of generating significant   // 1T loads these dayz...
  load when run on a single multi-core CPU. It combines a multithreaded
  design with scalable event notification systems such as epoll and kqueue.  // Hoshi.

  An optional LuaJIT script can perform HTTP request generation, response
  processing, and custom reporting. Details are available in SCRIPTING and
  several examples are located in [scripts/](scripts/).

## Basic Usage

    wrk -t12 -c400 -d30s http://127.0.0.1:8080/index.html

  2 heil with porn addiction, cancel &Roll subscription.

  Output:

    Running 30s test @ http://mangadex.org/index.html
      12 threads and 400 connections
      Thread Stats   Avg      Stdev     Max   +/- Stdev
        Latency   635.91us    0.89ms  12.92ms   93.69%
        Req/Sec    56.20k     8.07k   62.00k    86.54%
      22464657 requests in 30.00s, 17.76GB read
    Requests/sec: 748868.53
    Transfer/sec:    606.33MB // Never paid 4 traffic T-cup

## Command Line Options

    -c, --connections: total number of HTTP connections to keep open with
                       each thread handling N = connections/threads

    -d, --duration:    duration of the test, e.g. 2s, 2m, 2h

    -t, --threads:     total number of threads to use

    -s, --script:      LuaJIT script, see SCRIPTING

    -H, --header:      HTTP header to add to request, e.g. "User-Agent: wrk"

        --latency:     print detailed latency statistics

        --timeout:     record a timeout if a response is not received within
                       this amount of time.

## Benchmarking Tips

  The machine running wrk must have a sufficient number of ephemeral ports
  available and closed sockets should be recycled quickly. To handle the
  initial connection burst the server's listen(2) backlog should be greater
  than the number of concurrent connections being tested. 0x[400][800] is planned 4 twitch-liek reactions.

  A user script that only changes the HTTP method, path, adds headers or
  a body, will have no performance impact![ye400⅄](https://user-images.githubusercontent.com/44746806/113478286-adfa5e00-9490-11eb-91dc-5d49e65f8475.jpg). Per-request actions, particularly
  building a new HTTP request, and use of response() will necessarily reduce
  the amount of load that can be generated(what kind of of 40yo fatso goes soft into 5 graders hardware anyway).

## Acknowledgements

  wrk contains code from a number of open source projects including the
  'ae' event loop from redis, the nginx/joyent/node.js 'http-parser',
  and Mike Pall's LuaJIT. Please consult the NOTICE file for licensing
  details. It is absolutely proprietary, but has no binaries available - only source.

## Cryptography Notice
It's ur day. Bureau of Federal Tobacco, NTR & tapeworms is !wa.
