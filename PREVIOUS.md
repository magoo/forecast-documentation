# Previously Completed Forecasts
*Total*: 4  
*Average Brier Score*: 0.1424641081  

## Completed

### Fortune 500 Breach (October 2018)
Scenario: Will a Fortune 500 company appear in the Privacy Rights Clearinghouse data breach data in October 2018?    
Outcome: *More than one breach (48.35%) on Nov-06-2018*  
Score: `0.44451083`  
Discussion:  

This is the first forecast being run on structured breach data within the Privacy Clearing House. It is hitting a wide net (The Fortune 500) over a short time (October). Eleven panelists were able to download historic data and interpret trends over the years. Options for outcome are listed below with the current panel's forecast.

- No breaches. (19%)
- One breach. (32.65%)
- More than one breach. (48.35%)

### Chromium "Critical" (SEP2018)
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

### Struts (CVE-2018-11776)
Scenario: Will attacks exploiting the Apache Struts vulnerability (CVE-2018-11776) be observed by the community "in-the-wild?"  
Outcome: *Correct (34%) on Aug-27-2018*  
Score: `0.104`  
Discussion:  

  - This had problems with forecasters understanding "In The Wild"? Next time it will be bolstered to included honeypot activity, and differentiate between ITW vulns and ITW exploits.
  - Disclosed Aug-22-2018, PoC around Aug-26-2018, Exploitation Aug-27-2018
  - Calibration training is looking more important. Some forecasts were wild.
  - Wrote "[In The Wild](IN-THE-WILD.md)" documentation.

### NetSpectre
Scenario: Will attacks using NetSpectre’s methods be observed by the security community “in the wild”?  
Outcome: No  
Score: `0.021075`  
Discussion: https://medium.com/starting-up-security/forecasting-a-headline-risk-netspectre-3c60338fd596

## Ongoing

### NPM Package Compromise
Scenario: How many "malicious" advisories will NPM publish in December 2018?  
Outcome: TBD (Min: 0 Max: 2.7777777777777777) @ 90% confidence  
Score:   
Discussion:  
Nine panelists, with a 90% confidence interval estimate, estimate between `0 and 2.7` advisories about malicious NPM packages in December. This is probably the first "confidence interval" forecast with this panel and it seemed well understood without much explanation. To help inform the forecast, NPM has several years of advisory data that can be interpreted. This forecast was inspired by the NPM package breach impacting the copay wallet.

### Fortune 500 / GDPR
Scenario:  A Fortune 500 company is assessed a large fine for a violation of GDPR between November 15, 2018, and April 15, 2019.  
Outcome: TBD (Forecast Yes 47.08% / No 52.92%)
Score:   
Discussion:  
This was to measure the uncertainty of GDPR fines, since there is only reference class data to estimate with. Limitations included:

- Named target of fine must be a current member of Fortune 500 or a fully owned entity thereof
- Fine must exceed 1/5 of the maximum allowed GDPR fine to the Fortune 500 listed company

### Bloomberg "The Big Hack"
Scenario: Will the supply chain server hardware attacks described in the Bloomberg article be confirmed by Jan 1 2020?
Outcome:
Score:   
Discussion:  

This is based on the [Bloomberg "The Big Hack"](https://www.bloomberg.com/news/features/2018-10-04/the-big-hack-how-china-used-a-tiny-chip-to-infiltrate-america-s-top-companies) article and designed to inform a security team about upstream hardware compromise and _actual threats_ taking place outside of speculation. 20+ panelists.

- This will be confirmed. (Yes) `44.82%`
- This will not be confirmed. (No) `55.18%`

[Discussion can be found on Medium](https://medium.com/@magoo/forecasting-bloombergs-the-big-hack-16b41e0b182b).

### Blank!
Scenario:
Outcome:
Score:   
Discussion:  
