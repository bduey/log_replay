Legal Stuff:
These files are FREE; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; version 3.

These files are distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details

NEVER BLINDLY RUN ANY SCRIPT, CONFIG FILE OR APP WITHOUT FIRST VERIFYING IT WILL DO WHAT IS EXPECTED

Usage:
$scriptName --file <file_name> --server <server_address> [--delay <N>] [--port <port>] [--tcp]
  --delay <N> The number of milliseconds to wait between the replay of each message.
  --help      Print this help text and exit
  --file <file_name>      The file to read the syslog messages from.
  --no-echo   Do not echo the messages to the screen
  --no-loop   Do not replay the messages more than once.
  --no-ts     Do not change the timestamp before replaying the message.
  --port <port>      The port to connect to on the syslog server.
  --server <server_address>      The hostname or IP address of the server to send the messages to.
  --tcp       Use TCP instead of UDP.
  --version   Print this script's version and exit.\n");
**Examples:**
  #Send bluecoat sample logs to localhost on UDP\514 every 1 second: 
  ./syslog_replay.pl --file bluecoat.log --server 127.0.0.1 --delay 1000 --port 514
  Send bluecoat sample logs to 1.2.3.4 on TCP/514
  # syslog_replay.pl --file bluecoat.log --server 1.2.3.4 --port 514 --tcp

I have included some sample files (.log) of different types. Simply insert the one you'd like to use after the --file option.
