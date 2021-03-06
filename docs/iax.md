Here's a list of all IAX2 options that can be set in the `[general]` section
via the $iax_options parameter:

  * `bindport`: Bind Asterisk to this port. If you are binding to multiple
    addresses, you can specify the port for each interface in bindaddr (see
    below).

  * `bindaddr`: Make asterisk listen on the following IP addresses (can be used
    more than once). To specify the port on which an address should listen, add
    it after the address and a colon (e.g. '192.168.0.100:5554').

  * `iaxcompat`: Useful when you use layered switches.

  * `nochecksums`: Disable UDP checksums.

  * `delayreject`: Delay the sending of authentication reject to alleviate brute
    force attacks on passwords.

  * `amaflags`: Default AMA flag. It must be one of 'default', 'omit', 'billing',
    or 'documentation'.

  * `adsi`: Enable ADSI-compatible equipment.

  * `srvlookup`: Perform an SRV lookup on outbound calls.

  * `accountcode`: Default account for CDR.

  * `language`: Global default language for users.

  * `mohinterpret`: Default, preferred music on hold channel.

  * `mohsuggest`: Defaul, suggested music on hold channel.

  * `bandwidth`: Specify bandwidth of low, medium, or high to control which
    codecs are used in general.

  * `disallow`: Array of codec names to prevent Asterisk from using with IAX2.

  * `allow`: Array of codec names to allow Asterisk to use with IAX2.

  * `jitterbuffer`: Global default for enabling/disabling the jitter buffer (can
    be set per-user).

  * `forcejitterbuffer`: Force the use of the jitter buffer even if the other end
    has a poorly performing jitter buffer.

  * `dropcount`: Maximum number of frames to overlook (e.g. consider "too late")
    inside the last 2 seconds.

  * `maxjitterbuffer`: Maximum size for the jitter buffer.

  * `resyncthreshold`: Number of frames over twice the measured jitter after
    which a resync is performed.

  * `maxjitterinterps`: The maximum number of interpolation frames the
    jitterbuffer should return in a row.

  * `maxexcessbuffer`: Maximum size by which the jitter buffer can be over what
    is needed. After a period of high jitter, Asterisk will gradually lower the
    buffer to follow this maximum.

  * `minexcessbuffer`: Minimum amount of unused buffer.

  * `jittershrinkrate`: Number of millisecs by which to shrink the jitter buffer
    for each 20ms when buffer is too big.

  * `minregexpire`: Minimum amount of time (seconds) that can be requested as a
    registration expriation interval.

  * `maxregexpire`: Maximum amount of time (seconds) that can be requested as a
    registration expriation interval.

  * `encryption`: Enable IAX2 encryption.

  * `forceencryption`: Refuse to connect unencrypted.

  * `trunkmaxsize`: Maximum payload in bytes an IAX2 trunk can support at a given
    time.

  * `trunkmtu`: Maximum transmission unit for IAX2 UDP trunking.

  * `trunkfreq`: How frequently trunk messages are sent in milliseconds.

  * `trunktimestamps`: Whether to send timestamps for the individual sub-frames
    within trunk frames or not.

  * `iaxthreadcount`: Number of iax helper threads to handle I/O.

  * `iaxmaxthreadcount`: Number of extra dynamic threads that may be spawned.

  * `authdebug`: disable authentication debugging to reduce the amount of
    debugging traffic.

  * `tos / cos`: Settings for Quality of service. See Asterisk documentation in
    /usr/share/doc/asterisk-doc/asterisk.pdf.gz (from package asterisk-doc).

  * `regcontext`: dynamically created and destroyed NoOp priority 1 extension for
    a given peer who registers or unregisters with Asterisk.

  * `autokill`: Cancel transaction if we don't get ACK to our NEW within 2000ms.

  * `codecpriority`: Control the codec negotiation of an inbound IAX call.

  * `allowfwdownload`: serve out firmware to IAX clients which request it.

  * `rtcachefriends`: Cache realtime friends by adding them to the internal list.

  * `rtupdate`: Whether or not to send registry updates to database using
    realtime.

  * `rtautoclear`: Auto-Expire friends created on the fly on the same schedule as
    if it had just registered.

  * `rtignoreregexpire`: use the stored address information regardless of whether
    the peer's registration has expired.

  * `parkinglot`: Default parkinglot for IAX peers and users.

  * `calltokenoptional`: Set call token validation as optional.

  * `requirecalltoken`: Global setting for call token verification. Can be set to
    'no', 'auto', or 'yes'.

  * `maxcallnumbers`: Maximum amount of call numbers per IP before refusing new
    connections.

  * `maxcallnumbers\_nonvalidated`: Global maximum amount of call numbers before
    refusing new connections.

