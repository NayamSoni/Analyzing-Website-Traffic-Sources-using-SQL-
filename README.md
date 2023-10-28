Business Concept - Traffic Source Analysis

Traffic source analysis is about understanding where your customers are coming from and which channels are driving the highest quality traffic.  

Let's Start 

Topic 1: Finding Top Traffic Sources

SELECT 
      utm_source,
      utm_campaign, 
      http_referer,
      COUNT(user_id) AS Sessions
FROM website_sessions
     WHERE created_at < '2012-04-12'
GROUP BY utm_source,
         utm_campaign,
         http_referer;

Output: 

<img width="373" alt="image" src="https://github.com/NayamSoni/Analyzing-Website-Traffic-Sources-using-SQL-/assets/98815102/da35337e-3ea5-440e-b1ee-d6ef2e98fc09">


Conclusion: Based on the results I advised to focus on gsearch ( utm_source) and nonbrand (utm_campaign). Let's dig deeper into these fields.
