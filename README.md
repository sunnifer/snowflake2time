snowflake2time
==============

Converts Twitter snowflake ids to UTC timestamps (unix epoch seconds
or milliseconds) and back.

Snowflake Layout

1  sign bit -- not used, always 0?
41 bits (milliseconds since epoch) - 1288834974657L
5  bits datacenter id
5  bits machine id
12 bit sequence number


Currently in php and python.  Other languages welcome!


The Snowflake algorithm:

https://github.com/twitter/snowflake/blob/master/src/main/scala/com/twitter/service/snowflake/IdWorker.scala

Twitter IDs, JSON and Snowflake  2011-06-26
https://dev.twitter.com/docs/twitter-ids-json-and-snowflake

Other Snowflake news:

http://groups.google.com/group/twitter-development-talk/browse_thread/thread/5152a34a8ae6ccb6/1edb5cd6002f6499?pli=1

https://dev.twitter.com/blog/direct-messages-going-snowflake-on-sep-30-2011