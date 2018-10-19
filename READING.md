# Probabilistic Risk Assessment Reading Material 📚
This selection of reading is opinionated towards the work I am doing. Much of my learning has come from here, and the lessons help support the following goals:

1. First, adapting available tooling to measure risk despite how nuanced and fast moving the risks in cyber can be. This is mostly means forecasting for starters.
2. Second, organizing many risks and focusing teams towards the reductions of these risks through our tried and true best practices.
3. Third, making root causes and incident transparency forefront in the industry to make #1 less volatile and allow us to enter more typical reliability / safety engineering practices that reduce the load on a forecaster.

## Defining Risk: Variance of its use in practice and language.
The language of "risk" is highly flexible. Two people talking about "risk" may be speaking at each other entirely differently.

- https://plato.stanford.edu/entries/risk/#DefRis
- https://onlinelibrary.wiley.com/doi/pdf/10.1111/risa.12464
```

risk = an unwanted event which may or may not occur.
risk = the cause of an unwanted event which may or may not occur.
risk = the probability of an unwanted event which may or may not occur.
risk = the statistical expectation value of an unwanted event which may or may not occur.
risk = the fact that a decision is made under conditions of known probabilities (“decision under risk” as opposed to “decision under uncertainty”)

```

Other definitions are used frequently. For instance, lacking a popular mitigation (Driving with no seatbelt) or something at stake, subject to other threats (a position in a stock).

### Using very specific language for scenarios
"[The clarity test](https://en.wikipedia.org/wiki/Clarity_test)" is described [here](https://web.stanford.edu/class/cee115/wiki/uploads/Main/Schedule/DAPracticeAndPromise.pdf).


## Experts Estimating Things
This section generally appeals to how experts can be queried for quantitative data. The process of doing so, industrial examples, history of.

### Parimutuel betting ([link](https://en.wikipedia.org/wiki/Parimutuel_betting))
This describes the practice of gathering up forecast material and, typically, averaging it together. Further described in [Probabilistic Forecasts and Reproducing Scoring Systems](https://www.rand.org/pubs/research_memoranda/RM6299.html)

### Shigeru Myamoto's hobby of estimation
This is a humorous and extremely useful example of "being good at estimation". The creator of Super Mario regularly guesses the size and weight of objects, and carries around a tape measure to do so. This is a fantastic lead-in into the purpose of estimation.

- https://youtu.be/DiUeuc7eOh0?t=16s
- https://kotaku.com/5381876/miyamotos-secret-hobby-measuring-stuff

### All measurement is approximate
This section includes all references to, and arguments that measurements are estimates. Generally speaking, everything we do is some form of approximation, even when employing the use of measurement instruments.

- [Measurement in Science](https://plato.stanford.edu/entries/measurement-science/)

> "Although this may seem a paradox, all exact science is dominated by the idea of approximation." - Bertrand Russel

- The "How to Measure Anything" series has a significant section in defense of estimation. However, I wish this definition of measurement was more frequently stated elsewhere.

> "a quantitatively expressed reduction of uncertainty based on one or more observations"

The reference kilogram is the best example of measurement and estimation in reality. The most accurate weighing machine that exists is the Kibble Balance which weighs an object with an "electric kilogram"

- https://www.nist.gov/si-redefinition/kilogram-introduction
- https://www.nist.gov/si-redefinition/kilogram-kibble-balance
- https://www.wired.com/2013/01/keeping-kilogram-constant/
- https://www.engadget.com/2017/10/24/why-scientists-are-redefining-the-kilogram/
- https://en.wikipedia.org/wiki/Kibble_balance

> What is going to change is that with this redefinition, the uncertainties of fundamental constants is either going to go to zero," he said. "Or the uncertainties of the related fundamental constants is going to be drastically reduced."

International standards exist that agree that all measurement carries uncertainty. The [Joint Committee for Guides in Metrology](https://en.wikipedia.org/wiki/Joint_Committee_for_Guides_in_Metrology) represents this notion.

- [Evaluation of measurement data — Guide to the expression of uncertainty in measurement](https://www.bipm.org/utils/common/documents/jcgm/JCGM_100_2008_E.pdf)

> "All measurements are subject to uncertainty."

> "By international agreement, this uncertainty has a probabilistic basis and reflects incomplete knowledge of the quantity value."

### Calibration of Probabilities: The State of the Art
Very early paper on calibrated probability assessments.

> An important criterion for evaluating probability assessors is their degree of calibration. A probability assessor is well calibrated if, over the long run, for all statements assigned a given probability the proportion that is true is equal to the probability assigned. For example, if you are well calibrated, then across all the many occasions that you assign a probability of .8, in the long run 80% of them should turn out to be true. If, instead, only 70% are true, you are not well calibrated, you are overconfident. If 95% of them are true, you are underconfident.

- http://www.dtic.mil/docs/citations/ADA101986
- http://www.dtic.mil/docs/citations/ADA033248
- [PDF](files/a101986.pdf)
- [PDF](files/a033248.pdf)


### RAND, The Delphi Method, and Futures Methodology
RAND has been [developing methods](https://www.rand.org/pardee/pubs/futures_method/delphi.html) for expert estimation for decades.

- [Probabilistic Forecasts and Reproducing Scoring Systems](https://www.rand.org/pubs/research_memoranda/RM6299.html)
- [On the Epistemology of the Inexact Sciences](https://www.rand.org/pubs/reports/R353.html)
- [An Experimental Application of the Delphi Method to the Use of Experts](https://www.rand.org/pubs/research_memoranda/RM727z1.html)
- [The Systematic Use of Expert Judgment in Operations Research](https://www.rand.org/pubs/papers/P2795.html)
- [Convergence of Expert Consensus Through Feedback](https://www.rand.org/pubs/papers/P2973.html)
- [Improving the Reliability of Estimates Obtained from a Consensus of Experts](https://www.rand.org/pubs/papers/P2986.html)
- [The Use of the Delphi Technique in Problems of Educational Innovations](https://www.rand.org/pubs/papers/P3499.html)
- [Analysis of the Future](https://www.rand.org/pubs/papers/P3558.html)
- [Delphi](https://www.rand.org/pubs/papers/P3704.html)
- [Systematic Use of Expert Opinions](https://www.rand.org/pubs/papers/P3721.html)
- [Delphi Process](https://www.rand.org/pubs/papers/P3925.html)
- [Experiments in Group Prediction](https://www.rand.org/pubs/papers/P3820.html)
- [Predicting the Future](https://www.rand.org/pubs/papers/P3948.html)
- [Delphi and Values](https://www.rand.org/pubs/papers/P4182.html)
- [The Delphi Method](https://www.rand.org/pubs/research_memoranda/RM5888.html)
- [The DELPHI Method, II](https://www.rand.org/pubs/research_memoranda/RM5957.html)
- [The Delphi Method, III](https://www.rand.org/pubs/research_memoranda/RM6115.html)
- [The Delphi Method, IV](https://www.rand.org/pubs/research_memoranda/RM6118.html)
- [Experimental Assessment of Delphi Procedures with Group Value Judgments](https://www.rand.org/pubs/reports/R0612.html)
- [Comparison of Group Judgment Techniques with Short-Range Predictions and Almanac Questions](https://www.rand.org/pubs/reports/R0678.html)
- [Delphi Assessment](https://www.rand.org/pubs/reports/R1283.html)

### Expert elicitation in PRA
Start with [Expert elicitation](https://en.wikipedia.org/wiki/Expert_elicitation).

['Expert information' versus 'expert opinions.](https://www.sciencedirect.com/science/article/pii/095183209290023E) by [Stan Kaplan](https://www.risksciences.ucla.edu/testimonials/2015/1/22/testimonial-to-stan-kaplan) has a choice quote that is important to me. It illustrates the unpredictability of our risk and how methods can account for that unpredictability. Not every nuclear reactor has a snake problem, but a risk methodology should account for them if they exist. This is wholly anti-checkbox to me. See:

> During one such occasion, a wrench was, in fact, dropped into the vessel. One other occasion is known in which a small tool was dropped onto the vessel. All such events are included under this parameter. We must also include under this parameter the possibility of biological debris, i.e. the possibility that a small animal (small frog, large insect?) could come in through the hatch, hang up under the lid, and not be noticed. This may be far-fetched, but small snakes have been observed in the high bay and, once, in the pool itself.

Next, [Eliciting Probabilities from Experts in Complex Technical Problems](https://ieeexplore.ieee.org/abstract/document/83752/) is another scaled effort to gather expert opinion.
> The NRC subsequently funded a new and very extensive expert judgment process that used formal and explicit methods of elicitation and was thoroughly documented. Over 100 professionals were involved in this process which was headed by Sandia National Laboratories. We were involved, together with Professors Ward Edwards, Stephen Hora and Richard John, as consultants in the tasks of training experts and eliciting expert judgments.

### IARPA
IARPA invests in quite a bit of predictive research and publishes results often. They are also involved in forecasting tournaments.

- [Teams Better Than Individuals at Intelligence Analysis, Research Finds](https://www.iarpa.gov/index.php/newsroom/iarpa-in-the-news/2015/419-teams-better-than-individuals-at-intelligence-analysis-research-finds)

### Cooke's Method
Used in environmental / natural disaster forecasting (Volcanic, Earthquake, etc
- http://rogermcooke.net/rogermcooke_files/Automatica%201988%20Cal%20Inf.pdf
- https://academic.oup.com/reep/article/12/1/113/4835830
- http://www.rff.org/files/sharepoint/Documents/Features/294-295%20Opinion%20-%20Aspinall%20pr.pdf
- https://www.eeri.org/products-page/other-seminars-and-workshops/usgs-expert-elicitation-report/
- https://earthquake.usgs.gov/contactus/menlo/seminars/848
- https://earthquake.usgs.gov/static/lfs/nshm/workshops/GMPE2012/WED_AM01_Petersen.gmworkshop-berkeley-newsm.pdf


## Forecasting

### Philip Tetlock's prediction research
Tetlock's research I have been following revolves around how [experts who are untrained in prediction are worse than random](https://www.amazon.com/Expert-Political-Judgment-Good-Know/dp/0691128715). He has since isolated those who are stronger forecasters ([Superforecasters](https://www.amazon.com/Superforecasting-Science-Prediction-Philip-Tetlock/dp/0804136718)) and is identifying their qualities, especially around [how you make a better forecaster](http://journal.sjdm.org/16/16511/jdm16511.html). The [follow up use of teams](https://www.iarpa.gov/index.php/newsroom/iarpa-in-the-news/2015/439-the-good-judgment-project) is especially interesting.

- [Philip Tetlock](https://www.sas.upenn.edu/tetlock/)
- [Philip Tetlock Lecture](https://www.youtube.com/watch?v=xBXDTQdmNyw)
- [Writeup in New Yorker](https://www.newyorker.com/magazine/2005/12/05/everybodys-an-expert)

### Meteorology
Maybe the oldest area of forecasting. Understanding the industrial development of meteorology is a great rubric for how a predictive industry is built over time. First, the theory. Then the infrastructure. Then the operational practice of prediction, decision making, and learning.

- [Weather Analysis and Forecasting](https://www.ametsoc.org/ams/index.cfm/about-ams/ams-statements/statements-of-the-ams-in-force/weather-analysis-and-forecasting/)
- [Timeline of Meteorology](https://en.wikipedia.org/wiki/Timeline_of_meteorology)

### How to measure anything (series)
This is a fantastic defense of estimation and prediction with succinct examples of how subjective topics can be quantified. A very accessible approach to the subject.
 - [How to Measure Anything in Cybersecurity Risk](https://www.amazon.com/dp/B01J4XYM16)

## Scenarios
The development of scenarios seem critical for cyber security, as they are inherently probabilistic and are part of how `risk` is generally calculated.

I have been hunting for any school of thought that treats "scenarios" as hierarchal relationships. The earliest schools of thought in Computer Science I've been able to find go back to lectures in the late 80s by Edward Amoroso, who published an early book on computer security. Schneier appears in the 90's. This is clearly used in military contexts before both of them by "fault tree analysis". This is a fundamental aspect Probabilistic Risk Assessment.

- [Fault Tree Analysis](https://en.wikipedia.org/wiki/Fault_tree_analysis)

- [Attack Trees](https://www.schneier.com/academic/archives/1999/12/attack_trees.html)
- [Fault Tree Handbook with Aerospace Applications Version 1.1](https://elibrary.gsfc.nasa.gov/_assets/doclibBidder/tech_docs/25.%20NASA_Fault_Tree_Handbook_with_Aerospace_Applications%20-%20Copy.pdf)

### Fundamentals of Computer Security
The earliest record I have found of Fault Trees being used in a threat and computer security context.
- [Fundamentals of Computer Security](https://www.amazon.com/Fundamentals-Computer-Security-Technology-Amoroso/dp/0131089293)

### Intelligence Analysis
 [Intelligence Analysis](https://www.amazon.com/Intelligence-Analysis-Target-Centric-Robert-Clark/dp/1452206120) also spans the boundary of "thing that breaks" into a scenario, by deciding on specific future events to forecast. It has great language around thinking through scenarios that matter, and a full chapter of methods to decompose a scenario and plan it for consumption. This reading additionally supports forecasting and estimation in operational practice.

### Threat Modeling
Application threat modeling literature frustratingly avoids the probabilistic and quantitative nature of a scenario. Though, they thoroughly apply effort towards enumerating the causes of failures and mitigating them. So they are very useful for that knowledge. Addressing and improving into the probabilistic nature of threat models is an iteration that needs to happen.

- [Threat Modeling](https://www.amazon.com/Threat-Modeling-Microsoft-Professional-Swiderski/dp/0735619913)
- [Threat Modeling: Designing for Security](https://www.amazon.com/Threat-Modeling-Designing-Adam-Shostack-ebook/dp/B00IG71FAS/ref=mt_kindle?_encoding=UTF8&me=&qid=1535658874)

## Cognitive Error / Bias / Expert Failure

### Thinking Fast and Slow
[Daniel Kahneman](https://en.wikipedia.org/wiki/Daniel_Kahneman) and [Amos Tversky](https://en.wikipedia.org/wiki/Amos_Tversky) offer the most relevant research in this area. Their works reveal observations into how fallible the human mind is in the most common of circumstances. The classification of System 1 and System 2 thinking is highly relevant to this area of critical thinking around risk.

### Clinical versus Statistical Prediction
Paul E. Meehl and Robyn Dawes [work in prediction](https://en.wikipedia.org/wiki/Paul_E._Meehl#Clinical_versus_statistical_prediction) inspired a scientific full fledged assault on the credibility of expert prediction. Comprehensive findings that mechanical statistical models beat experts at prediction.

- [Statistical Prediction versus Clinical Prediction: Improving What Works](http://meehl.umn.edu/sites/g/files/pua1696/f/155dfm1993_0.pdf)
- [Clinical versus Statistical Prediction](https://www.amazon.com/Clinical-Versus-Statistical-Prediction-Theoretical/dp/0963878492/ref=sr_1_1?ie=UTF8&qid=1535672122&sr=8-1&keywords=clinical+vs+statistical+prediction&dpID=518VnLiicsL&preST=_SX218_BO1,204,203,200_QL40_&dpSrc=srch)

### Incerto (Esp: Fooled by Randomness / Black Swan)
This series, better than any other, explains the _difficulty_ of prediction and the misunderstanding and malpractice around randomness. It discusses the "Black Swan" with an eye towards our misunderstandings of unpredictable events. The largest takeaway is the concept of being "antifragile", which I have treated as shorthand for "Don't bother predicting everything, assume it will happen categorically."

An _antifragile_ look at cybersecurity for instance: spending all time and resource on prevention will guarantee poor incident response, while spending all time and resource on incident response might result in incidents...it will be better handled with better learnings and may be impressively handled and/or prosecuted.

-[Incerto: Fooled by Randomness, The Black Swan, The Bed of Procrustes, Antifragile](https://www.amazon.com/Incerto-4-Book-Bundle-Randomness-Antifragile-ebook/dp/B00K5190LE)

## Intelligence Processing

### Sherman Kent
[Sherman Kent](https://en.wikipedia.org/wiki/Sherman_Kent) is considered a pioneer of intelligence analysis, and brought probabilistic rigor into the National Intelligence Estimate.

- [Words of Estimative Probability](https://www.cia.gov/library/center-for-the-study-of-intelligence/csi-publications/books-and-monographs/sherman-kent-and-the-board-of-national-estimates-collected-essays/6words.html)
- [The Law and Custom of the National Intelligence Estimate](https://www.cia.gov/library/center-for-the-study-of-intelligence/csi-publications/books-and-monographs/sherman-kent-and-the-board-of-national-estimates-collected-essays/5law.html)
- [The Making of an NIE](https://www.cia.gov/library/center-for-the-study-of-intelligence/csi-publications/books-and-monographs/sherman-kent-and-the-board-of-national-estimates-collected-essays/making.html)
- [The Theory of Intelligence]( https://www.cia.gov/library/center-for-the-study-of-intelligence/csi-publications/books-and-monographs/sherman-kent-and-the-board-of-national-estimates-collected-essays/the-theory-of-intelligence.html)

### Canadian Intelligence
There is research around Canada's application of modern intelligence processing and its effectiveness. The basis of this is all probabilistic.

- [Canada Is Actually Pretty Good at Intelligence Forecasting](https://motherboard.vice.com/en_us/article/kbz7gn/canadian-intelligence-agencies-are-actually-pretty-good-at-strategic-forecasting)
- [Accuracy of forecasts in strategic intelligence](http://www.pnas.org/content/111/30/10984)

>  This study applied quantitative measures of forecasting accuracy commonly used in other areas of expert forecasting to over 1,500 strategic intelligence forecasts spanning approximately 6 y of intelligence production by a strategic assessment unit. The findings revealed a high level of discrimination and calibration skill.

## Blogging

### Twitch
> Predicting the future is not a theoretical superpower. It is a skill you are already using to make decisions, and like any other skill it can be rapidly improved with deliberate practice.

- https://hbr.org/2017/05/how-our-company-learned-to-make-better-predictions-about-everything
- https://blog.twitch.tv/why-im-teaching-twitch-to-predict-the-future-baeeafaf45f9

### Open Philanthropy Project
> In some cases, we need to make judgments about relatively tangible outcomes in the relatively near future, as when we have supported campaigning work for criminal justice reform. In others, our work relies on speculative forecasts about the much longer term, as for example with potential risks from advanced artificial intelligence. We often try to quantify our judgments in the form of probabilities — for example, the former link estimates a 20% chance of success for a particular campaign, while the latter estimates a 10% chance that a particular sort of technology will be developed in the next 20 years.

- https://www.openphilanthropy.org/blog/efforts-improve-accuracy-our-judgments-and-forecasts

### Kelly Shortridge

- [The Art of Explanation: Behavioral Models of InfoSec](https://www.youtube.com/watch?v=UdZDlt2dlqM)
- [Behavioral Models of InfoSec: Prospect Theory](https://medium.com/@kshortridge/behavioral-models-of-infosec-prospect-theory-c6bb49902768)


## Simulation / Tabletop / Red Team

### Red Teams
Fantastic, real world examples of theory in practice. For instance, a breakdown of multiple independent estimates that displayed a probability of Osama bin Laden living in a compound in Pakistan.
- [Red Team](https://www.amazon.com/Red-Team-Succeed-Thinking-Enemy/dp/0465048943/ref=sr_1_1?ie=UTF8&qid=1535661251&sr=8-1&keywords=red+teams&dpID=41627u1o5cL&preST=_SY344_BO1,204,203,200_QL70_&dpSrc=srch)

### Military Simulation / Operations Research
The use of tabletops, physical simulation, and predictive modeling off of historic data make up a significant amount of decision making in the military.

- [Military Simulation](https://en.wikipedia.org/wiki/Military_simulation)
- [War Games](https://www.amazon.com/War-Games-Creators-Players-Rehearsing/dp/0070011958)

- [Military Operations Research: Quantitative Decision Making](https://www.amazon.com/Military-Operations-Research-Quantitative-International/dp/0792398580/ref=sr_1_1?ie=UTF8&qid=1535661870&sr=8-1&keywords=military+operations+research)


## Industry
Industry examples where probabilistic risk assessment is at play:

- [NASA Risk Management Handbook](https://ntrs.nasa.gov/archive/nasa/casi.ntrs.nasa.gov/20120000033.pdf)
- [EPA: Risk Assessment Forum White Paper: Probabilistic Risk Assessment Methods and Case Studies](https://www.epa.gov/sites/production/files/2014-12/documents/raf-pra-white-paper-final.pdf)
- [Probabilistic Risk Assessment Procedures Guide for Offshore Applications](https://www.bsee.gov/sites/bsee.gov/files/ProbalisticRiskAssessment%20%28PRA%29/bsee_pra_procedures_guide_-_10-26-17.pdf)
- [Nuclear Probabilistic Risk Assessment](https://www.nrc.gov/about-nrc/regulatory/risk-informed/pra.html)

This paper has a specifically useful overview of many different industry approaches to safety.

> In addition, generalized probabilities and reliability analyses may not apply to specific,
localized areas: The probability of a bird strike causing an aircraft accident, for example, is much
higher at Midway Island than at most other places

This meets my criteria that is "anti-checklist". Safety engineering is good at surfacing and eliminating unique problem areas that are localized to a victim.
- [White Paper on Approaches to Safety Engineering](http://sunnyday.mit.edu/caib/concepts.pdf)

## Decision Science
This is a dumping ground for the various naming conventions of engineering areas that have come to accept quantitative reasoning.

- [Epidemiology](https://en.wikipedia.org/wiki/Epidemiology)
- [Process Optimization](https://en.wikipedia.org/wiki/Process_optimization)
- [Six Sigma](https://en.wikipedia.org/wiki/Six_Sigma)
- [Lean Manufacturing](https://en.wikipedia.org/wiki/Lean_manufacturing)
- [Kaizen](https://en.wikipedia.org/wiki/Kaizen)
- [TPS](https://en.wikipedia.org/wiki/Toyota_Production_System)
- [DFM](https://en.wikipedia.org/wiki/Design_for_manufacturability)
- [Quality Management](https://en.wikipedia.org/wiki/Quality_management)
- [Validated Learning](https://en.wikipedia.org/wiki/Validated_learning)
- [Taylorism](https://en.wikipedia.org/wiki/Scientific_management)
- [Operations Research](https://en.wikipedia.org/wiki/Operations_research)

---

## Looking for...

- Lessons where "cost of measurement" or over-measurement prevented an industry from succeeding.
- Deciding what to measure.
- More examples of industries that track incidents and failures religiously.
