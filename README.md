# pcap file format in Go

The format of the file is a `Header`, followed by `PacketHeader` and packet data pairs. `PacketHeader.IncludedLength` should match the length of the packet data to produce a valid file.

The headers should be binary encoded using either `encoding/binary` or [`github.com/iangudger/binary`](https://github.com/iangudger/binary).
