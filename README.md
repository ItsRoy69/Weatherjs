# Weatherjs

Skip to content
Search or jump to…

Pull requests
Issues
Marketplace
Explore
 
@ItsRoy69 
noazark
/
weatherjs.com
2
74
Code
Issues
Pull requests
1
Actions
Projects
Security
Insights
You’re making changes in a project you don’t have write access to. We’ve created a fork of this project for you to commit your proposed changes to. Submitting a change will write it to a new branch in your fork, so you can send a pull request.
weatherjs.com
/
README.md
in
noazark:gh-pages
 

Spaces

2

Soft wrap
1
Weather.js
2
==========
3
​
4
[![Build Status](https://secure.travis-ci.org/noazark/weather.png?branch=master)](https://travis-ci.org/noazark/weather)
5
​
6
## About
7
​
8
There really should be a conclusive Javascript weather library.
9
Weather.js fetches data from [openweathermap.org][] (no affiliation).
10
Since other providers format their output differently, currently this is
11
the only source provider.
12
​
13
Weather.js is still in early development so expect changes and please
14
contribute! Among the features I hope to incorporate:
15
​
16
-   historical weather information
17
-   API key usage
18
-   more data sources
19
-   more conversions!
20
​
21
​
22
## Install
23
​
24
Weather.js works in the browser and node.js. Take your pick. For the
25
browser, [download the most recent version on github][Weather.js]. For use in
26
node, do the install thing.
27
​
28
```
29
npm install -g weather.js
30
```
31
​
32
**Important!** In the browser you will need to also include [Sugar.js][]
33
and [jQuery][]. I will try to remove these dependancies as soon as
34
possible.
35
​
36
## Usage
37
​
38
At the moment you can access the current weather conditions and the
39
forecast for any city. By default it will use the closest match as
40
returned by Open Weather Map.
41
​
42
```javascript
43
Weather.getCurrent("Kansas City", function(current) {
44
  console.log(
45
    ["currently:",current.temperature(),"and",current.conditions()].join(" ")
46
  );
47
});
48
​
49
Weather.getForecast("Kolkata", function(forecast) {
50
  console.log("forecast high: " + forecast.high());
51
  console.log("forecast low: " + forecast.low());
52
});
53
```
54
​
55
[openweathermap.org]: http://openweathermap.org
56
[Weather.js]: http://github.com/noazark/weather
57
[Sugar.js]: http://sugarjs.com/
58
[jQuery]: http://jquery.com/
No file chosen
Attach files by dragging & dropping, selecting or pasting them.
@ItsRoy69
Propose changes
Commit summary
Create README.md
Optional extended description
Add an optional extended description…
 
© 2021 GitHub, Inc.
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
