---
author: Patrick Zandl
categories:
- AI
lang: en
layout: post
original_lang: cs
post_excerpt: "We have just experienced two very instructive events that have helped us better understand the dangers posed by AI. It brings _post-truth_—a complete imitation of knowledge that lacks the one thing it needs: knowledge. Everything else is in place. I was sitting in the front row, so I’ll give you a report."
thumbnail: https://www.marigold.cz/assets/nehoda-ai-agenta.png
title: 🏄🏻‍♂️ The post-truth world: lessons from the blackout, the Pope, AI, and our brains
---


We have just experienced two very instructive events that have helped us better understand the dangers posed by AI. It brings  **_"post-truth"_**—a complete imitation of knowledge that lacks the one thing it needs: knowledge. Everything else is in place. I was sitting in the front row, so I'll give you a report.

When, on April 28, 2025,  [the power grid went down on the Iberian Peninsula](https://www.marigold.cz/item/spanelsko-blackout/), the internet was soon filled with speculation, as is usually the case. But just a few hours after the outage, the first comprehensive studies of what had happened also appeared. And that was strange. At such a moment, it is quite common among laypeople to have an opinion or an initial reaction based on anecdotal observations, i.e., on the perception of an isolated phenomenon. As a rule, people who are knowledgeable about energy do not have such opinions, because they know very well that the system is complex and that authoritative statements such as "XY is to blame" will inevitably be laughed at later. Besides, at that moment, it is not important for energy experts WHAT happened, but HOW to get out of it—how to restore supplies. These are, at least at that moment, two completely different things.  

It was therefore striking that comprehensive materials on what had happened appeared soon after the outage, primarily on LinkedIn. I can mention James Cupps and his report  [Technical Analysis of Spain's Power Grid and the April 28, 2025 Outage](https://www.linkedin.com/pulse/technical-analysis-spains-power-grid-april-28-2025-outage-james-cupps-palff/)  from the afternoon of April 28, 2025, just a few hours after the outage. Many websites analyze the architecture and condition of the Spanish distribution network and the causes of the blackout in great detail. Cupps must have put a tremendous amount of work into the report, or he must have had it partially done by chance and was able to quickly finish his analysis of the blackout. Except that he didn't. James Cupps is not an energy expert at all, and the report was written by the ChatGPT model o3 for his LinkedIn newsletter  [Experiments using AI chatbot](https://www.linkedin.com/newsletters/7020788143490555906/), in which Cupps publishes comprehensive "reports" on current topics written by ChatGPT's deep research mode. In addition to energy, he has regaled us with a profile of the new Pope Leo XIV and an analysis of the Commvault CVE-2025-3928 vulnerability. Cupps is thus generating interest in his consulting firm's LinkedIn profile, and the Spanish blackout was a godsend for him because he found a number of subscribers.  

You may ask why it matters who the author is... Well, because Cupps' "technical analysis" contains a number of factual errors. However, only someone familiar with the Spanish transmission network will spot them. Otherwise, he has everything: credible-looking, highly detailed, and technical claims that appear to be irrefutable arguments. Yet the text is riddled with inaccuracies and AI hallucinations. For example: "REE also manages high-voltage distribution for Portugal based on agreed mechanisms because the systems are synchronized (although the Portuguese distribution network is owned by REN)." This is patently untrue. The Spanish REN has no direct dispatching access to the Portuguese grid. REE (Spain) and REN (Portugal) work closely together and coordinate the operation of the Iberian Power System (MIBEL), but REN is responsible for dispatching the Portuguese transmission network. An energy expert would not have made such a simplification, because they know that this difference matters, but LLM does not consider it a significant difference.  

There are many similar minor errors in the text. The connection between Spain and Morocco is stated in the text as 700-900 MW, but this is more of an average usage, and the capacity is actually around 1400 MW. LLM could easily make this mistake. Similarly, the statement that "Spain has essentially ended coal-fired power generation" could be considered hyperbolic, as the country still has approximately 3 GW of capacity available, which it uses for stabilization.

Of course, one could argue that these are minor details, but they are significant and there are quite a few of them. Each one on its own could be explained away and dismissed with a wave of the hand. But when you add up all the errors in the text, you end up with a significant difference in the quantitative parameters of the grid, which means that the report draws conclusions that it simply has no basis for. Unfortunately, in a grid, the order matters a lot, i.e., what was the cause and what was the effect, because both are dealt with differently and very expensively.

The result? The report looks professional, but in reality it has no value. However, you won't notice this at first glance, or even at second glance, or subsequent glances. It has all the trappings to convince laypeople. It uses the correct technical language, the correct formatting, specific figures, and conclusions that appear credible at first glance. However, it was not based on the underlying data, because that data did not yet exist at the time. And so it gave a completely convincing answer to a question that could not yet be asked.  

I myself have verified how dangerous and seductive this is. In the first moments after the blackout, I accepted the statement that one of the outages was caused by an atmospheric phenomenon. Although I have a decent understanding of how the transmission network works, I had to ask AI to explain the effect of temperature gradients on cable vibrations. It explained it to me very convincingly, but in one case it exaggerated the temperature differences and in another it underestimated them, so the problem seemed plausible. In reality, the temperature differences were not significant at the time in question and the cable vibrations could not have had any effect, but because the news was constantly being repeated by the agencies, it took me until the next day to dismiss the idea as implausible.

### AI and why wasn't the expected pope elected?  

The second similar example was the election of the pope. Apparently, a number of people thought it would be a good idea to enter a simple prompt, turn on deep research, and post the answer on social media as a profound spiritual reflection. However, Robert Prevost, who was elected Pope Leo XIV, did not even make it to the list of dark horses in any of these models, let alone the list of candidates under consideration.  

_I chose this example because I know a little about it. First, I studied this topic in college, so I am familiar with the conclave process and realize how different it is from other types of elections. There are no reliable pre-election polls for the election of a pope, and the process is shrouded in secrecy._  _Second, last year we developed an AI tool for mapping risks in decision-making processes, which in theory can also be used to predict the "future," for example, to map the probabilities of the election of a new pope._  

AI cannot predict the future in any way. It can take large amounts of data, sort it in various ways, and draw conclusions from it. It can find turning points and extend trends. But it certainly cannot do this with a single prompt to ChatGPT. You have to be aware of what you know. And also what you don't know.  

The fundamental problem with the election of Prevos as pope was what we did not know. Let's now recap his election as predicted by

When estimating the conclave, it is necessary to first follow a "network model," i.e., consider the level of support each candidate has. This is usually done by closely monitoring which institutions and associations the cardinal in question belongs to, who he sits next to at press conferences, etc. The reasoning is that candidates who have the most colleagues "they get along with"—i.e., who they know personally and who are not controversial to them—have the best chance. The network model is actually quite comprehensive, and my model considered Pietro Parolin to be the most promising candidate, who I thought would get about 45 votes in the first round (out of 133 electors, with 89 needed to be elected). Parolin did indeed receive this number of votes in the first ballot on Wednesday, with Tagle receiving 32 votes, Zuppi 20, Prevos 15, and the others 21. It was expected that there would be a reshuffle until the end of the day and that Parolin would strengthen his position, but in the final vote on Wednesday, he apparently received only around 50 votes and did not gain any more. Tagle and Zuppi lost ground, and the only one who gained was Prevost. He apparently caught up with Parolin in the second vote on Wednesday (although some sources mention only one vote on Wednesday).  

This was followed by night-time negotiations, and in two votes on Thursday, Prevost was deemed "acceptable" and received 101 votes, which was comfortably enough to secure his election. He gained votes mainly from Tagle and Zuppi's supporters and some conservatives. A factual note here: no official report other than "elected" has been released from the conclave—all figures are from articles by AP, ABS, Sky, and El Pais, which cite some "insiders." and the numbers sometimes differ (Parolin could have reached up to 55 votes) – but that is not important. What is important is the ceiling at which he got stuck and the shift of support to Prevost, on which they agree.

Why did neither AI nor any media polls pick up on Prevost with such a strong mandate? How could he have escaped the bookmakers?  

In both cases, it's about timing. Prevost was certainly not insignificant, but he only became a cardinal in September 2023, nine months before he became prefect of the Dicastery for Bishops, the institution with the greatest influence on the selection of bishops. Of course, bishops do not vote, but Prevost was in fairly close contact with about 70 cardinals regarding the selection of bishops. In other words, with the electors. This and several other similar positions he has held in recent years suggest that this was a deliberate and long-term strategy on the part of Pope Francis. He did not become a cardinal-bishop until February 2025, making him one of the highest-ranking church officials and one of the five members of the council assisting the pope—as well as one of the five who elect the dean who convenes the conclave.  

This role has not yet been picked up by general AI models, most of which have data up to mid-2024, when Prevost was not yet among the highest-ranking members of the Church.

Prevost has risen rapidly in recent months in invisible Church roles that signify influence, and it was not until February 2025 that he reached another visible milestone.  

Why did the media and bookmakers fail to pick up on Prevost's rise? Probably because public discussions favor cardinals with visible dioceses (Rome, Manila, Bologna). Prevost managed the church  _process_, not the "show," and therefore escaped the radar of commentators.  

And the taboo of electing an American? The "no American" taboo was broken by the fact that most of the electors from the US come from immigrant families and see themselves as part of the global South. But Prevost spent 30 years in Peru and speaks fluent Spanish, so he was seen as acceptable to both the US and Latin America. After all, Peru celebrates him as "its pope."

In the end, the dynamics of the conclave clearly worked. In the event of a stalemate, votes typically shift toward a compromise. Simulations considered  _rather one_ shift window. Reality showed  **two waves**  and a rapid snowball effect on Thursday morning. This was probably also because Prevost was the first logical and dignified choice during the stalemate, with growing support for the weary cardinals.  

To be honest, I wanted to include a warning in my prediction that if the conclave did not proceed with steady growth in the first round, it would be the turn of the dark horses, but I was betting more on the Patriarch of Jerusalem, Pierbattista Pizzaballa. Prevost also flew under our data analysis radar, as we had not collected any data for this year. This is a rather significant error in data analysis :(

### We will be encountering AI analyses more and more often  

We will encounter them more and more often as editors try to save even more money while offering "attractive content." After all, no one predicted the pope, so who cares who got it wrong? The thing is, if a human had done the analysis, they would have quickly concluded that the group could be narrowed down, but it would be impossible to predict who it would be. My software calculated that the probability of Parolin being elected is about 28%, but I found that number so specific that I almost believed it. And that's the thing. AI can communicate so convincingly that it gives us certainty, but often false certainty. It gives us the feeling that we understand something we don't understand at all, even with its help.  

What does this mean for the future? I have implicitly trained my ChatGPT to give me accurate and factual information and not to engage in speculation without my prompting.

### How can you recognize AI analysis?  

This will be an increasingly common problem.

1.  It is striking when, shortly after an unexpected event, an authoritative and, at first glance, carefully prepared comprehensive document containing a wealth of details emerges. Let alone when it is in Czech.  
    
2.  The author of the material is identified as someone who does not work in the field and has no knowledge or expertise in the area—for example, you should not primarily trust my assessment of the papal election because you do not know that I studied religious studies.  
    
3.  The most characteristic feature is the uniform syntactic and lexical structure, showing high grammatical consistency with minimal stylistic variability. The text usually contains extremely precise terminology without personal anecdotes or contextual digressions, suggesting a generative compilation from database knowledge rather than individual experience. (Yes, this point was generated by AI.)  
    
4.  When the text is free of emotional coloring, evaluative elements, or allusions and jokes, or when all citations are marked consistently—most people no longer remember from school how to cite sources in university papers—accurate, neutral, sterile text is a sign of AI.  
    
5.  If frequent probabilistic assessments such as "unlikely" or "most likely" are used, this indicates the use of LLM probabilistic classification, not the author's warm relationship with the probability scale.  
    

### And how will the media come across this?

First and foremost, we need to return to the good old journalistic practice of verifying information. Don't get me wrong, AI is certainly a valuable aid in creating the skeleton of an analysis, but it takes a lot of human experience to decide which of AI's suggestions are good and which are not. This will require not only a person with a good knowledge of the problem being described, but also an understanding of the limits of AI. In general: in current information that you have not explicitly instructed them to find on the web and in topics that are poorly researched or described on the web. For example, I have a decent idea of the limits of AI, but if it generates a report on a hockey championship, I cannot verify it.  

However, it may also be that users will not mind. That they will not find AI-generated reports bad. That pretending to know will be the same as knowing for them.

_And that is the age of post-truth..._