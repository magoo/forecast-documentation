# Previous Forecasts
*Total*: 3  
*Average Brier Score*: 0.0417818675  

## Chromium "Critical" (SEP2018)
Scenario: Will a "Critical" Chromium exploit be discovered "in the wild" in September 2018?  
Outcome: *Correct (98.36%) on Oct-02-2018*
Score: `0.0002706024999999994`
Discussion:

`Yes.` came in at `1.64%`, which suggests a future with all things being stable, a "Critical" exploit to occur once every five years given the current known universe. Forecasters were extremely positive on Chrome's security posture given its history, its current investment, and the current rate of Critical bug findings which occur around 0-4 times a month and always discovered under ideal circumstances.

All forecasters felt that leaving at least minimal (`<1%`) odds for a surprise event was adequate. The more liberal forecasters went up to 5% and claimed circumstances outside of Google's control that might release a known exploit into the wild. Those were Brexit, Russia and North Korea hacking, Midterm elections. Further opposition to this claims that news media has little to do with burning 0day, as the most important stuff is generally individualized and opportunistic, unlikely to be used where attention is pointed.

Small amounts of uncertainty came from the possibility that exploits have been in the wild and not reported on, or under gag order, but this is compared with how newsworthy it would be making it unlikely to be secret for long.

There was strong debate about whether events or potential "exploit hoarding" mattered or even takes place for Chrome. Those who forecasted higher odds were in strong agreement that if these events _were not_ taking place, they would have forecasted `<1%` odds, putting a "critical" bug rate around once every eight to thirty years if forecasts fell in that range.

  - Panel included 15 very reputable information security professionals and one PHD research scientist with a statistics background.
  - This is the first forecast to have data prepared for participants (prepared Chromium bug data and CVE data)
  - First attempt to include some basic modeling for forecasters (output of a hacky Markhov Chain Monte Carlo)
  - First to include expert interview data for forecasters. (Q&A with a former Googler familiar with Chrome)
  - I observed that new forecasters have trouble with sub 1% predictions, and shared guidance on how probability in this case can be described as a monthly frequency (1 month per decade, etc).
  - Without the current political climate, several forecasters would put `Yes` at 1% or lower, which could be useful for a follow up forecast?
  - Not all participants are trained, and some are new to forecasting, which will increase noise.
    - I wrote a training document as a result of this. ([TRAINING.md](TRAINING.md))
  - Gathering data for this was a "real job" and took a day of effort for one person (me). This forecast collected submissions over a two day period. About half of the forecasters updated their positions based on discussion. Some as drastically as 10%.

## Struts (CVE-2018-11776)
Scenario: Will attacks exploiting the Apache Struts vulnerability (CVE-2018-11776) be observed by the community "in-the-wild?"  
Outcome: *Correct (34%) on Aug-27-2018*  
Score: `0.104`  
Discussion:  

  - This had problems with forecasters understanding "In The Wild"? Next time it will be bolstered to included honeypot activity, and differentiate between ITW vulns and ITW exploits.
  - Disclosed Aug-22-2018, PoC around Aug-26-2018, Exploitation Aug-27-2018
  - Calibration training is looking more important. Some forecasts were wild.
  - Wrote "[In The Wild](IN-THE-WILD.md)" documentation.

## NetSpectre
Scenario: Will attacks using NetSpectre’s methods be observed by the security community “in the wild”?  
Outcome: No  
Score: `0.021075`  
Discussion: https://medium.com/starting-up-security/forecasting-a-headline-risk-netspectre-3c60338fd596
