


Scrappy
=======

![Scrappy Logo](Scrappy - small.png)

If you want to automate tasks in the web, this is your go to library. It uses CsQuery to parse html and ModernHttpClient for session management. 

Features:

* Form-Handling
* Link-Handling
* Header-Mimicking
* HTML-Parsing and CSS-Selectors using [CsQuery][1]

####Usage####

Simple sample fetching my IP from whatsmyip.org:
```csharp
var browser = new Browser();

var page = await browser.Open("http://www.whatsmyip.org/");

var myIp = page.Select("#ip").InnerText;

```


####Samples####

[WolframCalculator][s1]: Commandline tool which sends an expression to wolframalpha.com and displays the plain-text result to the user.


####Planned Features####

* Resource downloader and management
* Reactive extensions
* Javascript interpreter


[1]: https://github.com/jamietre/CsQuery

[s1]: https://github.com/Manuel-S/Scrappy/blob/master/Samples/WolframSample/Program.cs
