DerelictVorbis
==========

A dynamic binding to [libvorbis][1] for the D Programming Language.

Please see the pages [Building and Linking Derelict][2] and [Using Derelict][3], in the Derelict documentation, for information on how to build DerelictVorbis and load libvorbis at run time. In the meantime, here's some sample code.

```D
import derelict.vorbis.vorbis;
import derelict.vorbis.enc;
import derelict.vorbis.file;

void main() {
    // Load the libvorbis library and its companion encoding and file libaries.
    DerelictVorbis.load();
    DerelictVorbisEnc.load();
    DerelictVorbisFile.load();

    // Now libvorbis functions can be called.
    ...
}
```

[1]: http://xiph.org/vorbis/
[2]: http://derelictorg.github.io/compiling.html
[3]: http://derelictorg.github.io/using.html