This library provides a simple interface for generaing a few ANSI control
sequences for prettier serial screen displays.

1. Create a "wrapper" around a stream device:

    ANSI ansi; // Default Serial
    // or:
    ANSI ansi(Serial3); // Select a serial port

2. Generate ANSI sequences.  At the moment only clear screen and set cursor are supported:

    ansi.cls();
    ansi.setCursor(3, 2);

