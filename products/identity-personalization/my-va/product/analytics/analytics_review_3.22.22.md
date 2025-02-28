# My VA analytics review 

Notes from 3.22.22

## Reports referenced

All reports are from 7.1.22 (around when the 2.0 design launched) to 3.21.22

- [My VA analytics dashboard](https://analytics.google.com/analytics/web/#/dashboard/XOEdSZeVT9qyxQU5T29PNw/a50123418w177519031p176188361/_u.date00=20210701&_u.date01=20220321/)
- [My VA interactions](https://analytics.google.com/analytics/web/#/report/content-event-pages/a50123418w177519031p176188361/_u.date00=20210701&_u.date01=20220321&explorer-table.plotKeys=%5B%5D&explorer-table.rowStart=0&explorer-table.rowCount=25&_r.drilldown=analytics.pagePath:www.va.gov~2Fmy-va~2F,analytics.eventCategory:Interactions/) (**Note**: These numbers slightly differ from the aggregate data on the analytics dashboard because they are for /my-va/ only and don't include all URLs that include /my-va/)
- [Searches initiated from My VA](https://analytics.google.com/analytics/web/#/report/content-site-search-pages/a50123418w177519031p176188361/_u.date00=20210701&_u.date01=20220321&explorer-table.plotKeys=%5B%5D&explorer-table.rowCount=50&_r.drilldown=analytics.searchStartPage:www.va.gov~2Fmy-va~2F/)
- [VA.gov homepage interactions](https://analytics.google.com/analytics/web/#/report/content-event-pages/a50123418w177519031p176188361/_u.date00=20210701&_u.date01=20220321&_r.drilldown=analytics.pagePath:www.va.gov~2F,analytics.eventCategory:Interactions&explorer-table.plotKeys=%5B%5D&explorer-table.rowStart=0&explorer-table.rowCount=25/)

## Notes

- "View your profile" is the top click.
- Claim info, as expected, is also a primary action. I think we've placed it on the page accordingly.
- Surprisingly high rankings for clicking in "What benefits does the VA offer" and the education benefit application. Both rank higher than all health care links.
- Health care interactions almost don't make the top 10. Going to MHV via the main nav is #10, followed by clicking into messages (#12). This mirrors what we see on the VA.gov homepage. Health care interactions rank lower than viewing claims, viewing payments, and downloading letters. This might change as the health apartment grows, but makes sense right now given that most health care users sign in directly to MyHealtheVet.
- With regards to search, most of the the top 10 search terms are things we're about to add to My VA -- payment info, debt info, and a link to direct deposit. This will likely change once that work launches, as we've seen drops in all searches for things we've added to My VA (eg. disability rating, elevating claim status, link to travel pay). 
- Besides the aforementioned searches for payment/pay, debts, and direct deposit (and travel pay, which was recently added to My VA), there are only a small handful of other terms that round out the top searches since July:
  - **Top 10**: dependents, letters, DD214
  - **Top 25**: Variations on dependents and letters, COE/certificate of eligibility, GI Bill, ID card

## Questions

- Why is "View your profile" the top click? Do people expect to see info on My VA that they do not? Or do people need to make profile updates?
- If we moved up "You have n unread messages," would more people get to their health care inboxes faster? Do we care about this right now?

## Thoughts

- We will likely see a jump in interactions after we point users logging in from the homepage to My VA. It may be worth waiting to get analytics from that before determining how we might restructure things.
- Given that most health care users go straight to MHV for their health care information, I don't think we need to do a bunch of experiments or efforts to get people to click health care links more. Clicks into these links will probably increase (1) when we point to My VA for people logging in from the homepage and (2) as the health apartment work ramps up.
- Right now, there isn't actually that much on the My VA page. Adding the payments section certainly improves that, but an experiment restructuring the data make not actually be that helpful right now.
- Based on the data, it might be helpful to add a records section, given the frequency of searches for letters, DD214, and ID cards.
