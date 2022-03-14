# regex

Returns values containing URLs ending with favicon.ico.
(?<favicon>(?:https?\:\/\/|www\.)(?:[-a-z0-9]+\.)*[-a-z0-9]+\/favicon\.ico)
  
Returns values in URLs that may be keywords when searching Amazon.com as of 03/13/2022.
(?<amz>(?<=s\?k\=)[\w \+]+)

Returns a youtube URL
(?<yturl>^[^&]+)
