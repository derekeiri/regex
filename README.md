# regex

A handful of regular expressions that I found useful when reviewing logs of URLs, i.e., proxy.

Returns values containing URLs ending with favicon.ico.
```
(?<favicon>(?:https?\:\/\/|www\.)(?:[-a-z0-9]+\.)*[-a-z0-9]+\/favicon\.ico)
```

Returns values in URLs that may be keywords when searching Amazon.com as of 03/13/2022.
```
(?<amz>(?<=s\?k\=)[\w \+]+)
```

Matches a youtube video link.  For my use case, I would compile a list of youtube URLs and use Magnet Web Page Saver to generate the web page title. I can then generate/summarize a list from the HTML report.
```
^.*youtube.com\/watch\?v\=.*
```
