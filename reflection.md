The largest difficulty I faced in development is using tables. They can be very tedious as a nested structure and themselves have multiple elements with 1-letter differences (tr, td...). What helped me was recalling the full names for them to remember their purpose: table header, table data, etc.

It was also a challenge to try to create a sort of pixel art with empty but colored table data cells, which I made a lot less repetitive by using table colspans when I had rows of the same color.

The transfer from my local computer to our Linux server on my account would take a while. I was also unsure about how to transfer images to our server. The way I did this was by creating a new setup for SFTP and connecting a local folder to my public_html, then doing a local-to-remote sync which transferred everything from that local folder root directory.

Another issue was nginx permissions. I had to look up what chmod is and what the numbers mean. What got mine to display was the command: chmod 755 public_html. Each number has a meaning, the first 7 means the owner can read/write/execute, the second 5 means groups can read/execute, and the third 5 means others can read/execute.