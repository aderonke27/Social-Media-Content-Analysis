# Social-Media-Content-Analysis

## Table of Contents
1. [Project Overview](#project-overview)
2. [Problem Statement](#problem-statement)
3. [Objectives](#objectives)
4. [Dataset Description](#dataset-description)
5. [Tools Used](#tools-used)
6. [Data Cleaning Process](#data-cleaning-process)
7. [Data Analysis](#data-analysis)
8. [Dashboard](#dashboard)
9. [Key Insights](#key-insights)
10. [Recommendations](#recommendations)
11. [Limitations](#limitations)
12. [Conclusion](#conclusion)
13. [Project Files](#project-files)
14. [Contact Information](#contact-information)

## Project Overview
This project presents a comprehensive social media content performance analysis across six major platforms — YouTube, TikTok, Instagram, X.com, LinkedIn, and Facebook — using Microsoft Excel. The dataset covers 5,600 posts spanning multiple regions, content types, and post formats, capturing a wide range of engagement, reach, and audience interaction metrics.

The goal of this analysis was to identify which platforms, content categories, post types, regions, and time slots drive the highest engagement — enabling data-driven decisions around content strategy, posting schedules, and audience targeting to maximise social media performance.

## Problem Statement
Brands and content creators publishing across multiple social media platforms face a significant challenge: without a structured view of what content performs best, where, when, and for whom, resources are wasted on low-performing strategies while high-impact opportunities are missed.

This analysis addresses that challenge by examining 5,600 posts across six platforms and eight global regions to uncover which content formats, categories, and time slots consistently drive the strongest engagement and impressions.

## Objectives
* Evaluate total engagement, views, likes, shares, and comments across all platforms
* Identify which platforms generate the highest audience engagement
* Determine which content categories and post types perform best
* Analyse regional performance to identify where audiences are most active
* Uncover peak posting times and days for maximum reach
* Compare organic versus sponsored content performance
* Deliver strategic recommendations to improve content planning and social media ROI

## Dataset Description
The dataset contains 5,600 social media posts published across six platforms and eight global regions, with each record capturing a comprehensive set of performance metrics and post attributes.

The Post_ID field uniquely identifies each post, while Platform specifies the social media channel — YouTube, TikTok, Instagram, X.com, LinkedIn, or Facebook. The Content_Type field distinguishes between organic and sponsored posts, and Content_Category classifies each post by purpose — including Product Promotion, Educational, Entertainment, Customer Story, and Event/Webinar content. The Post_Type field captures the format of each post, covering Video, Image, Carousel, Live Stream, Text, Article, and PDF formats.

Geographic fields include Region, Longitude, and Latitude, covering posts from the USA, UK, India, Brazil, Australia, Canada, Germany, and Japan. Core engagement metrics include Engagement (total interactions), Views, Likes, Shares, and Comments, with Engagement_Rate expressing interaction as a proportion of reach. Reach and visibility are captured through Impressions, Video_Views, Live_Stream_Views, and Clicks, with the Click_Through_Rate field measuring how often viewers took action after seeing a post.

Time-based fields include Post_Published_At, Post_Date, Day_Name, Post_Hour, and a derived Column2 time slot field (e.g. 8am–10am, 11am–1pm) that enables time-of-day analysis. The Main_Hashtag field records the primary hashtag used per post, and Engagement_Level classifies each post's performance as Low, Medium, or High.

## Tools Used
Microsoft Excel

## Data Cleaning Process
Before analysis, the dataset was reviewed and prepared to ensure accuracy and consistency:
* Date and time formatting — Post published dates were stored as serial numbers and were converted to readable date formats. The Post_Hour field was used to derive time slot categories for time-of-day analysis
* Column labelling — Generic column names (Column1, Column2) were reviewed and relabelled based on the values they contained to improve clarity during analysis
* Data type validation — Engagement metrics, rates, and coordinate fields were verified and formatted correctly for aggregation in PivotTables
* Engagement Rate and Click-Through Rate formatting — Values stored in scientific notation were converted and formatted as percentages for readability
* Missing values — Fields such as Clicks, Click_Through_Rate, Video_Views, and Live_Stream_Views contained blank entries for non-applicable post types (e.g. text posts have no video views), which were reviewed and excluded from relevant calculations rather than treated as errors
* Engagement Level classification — The Engagement_Level field (High, Medium, Low) was verified for consistency and used as a key segmentation variable throughout the analysis

## Data Analysis
The analysis was structured across six key dimensions:
* Platform Performance: Total engagement, views, and impressions were aggregated by platform to identify which channels deliver the highest audience interaction and reach.
* Content Category Analysis: Posts were grouped by content category — Product Promotion, Educational, Entertainment, Customer Story, and Event/Webinar — to determine which types of content consistently drive the most engagement.
* Post Type Analysis: Performance was compared across post formats — Video, Image, Carousel, Live Stream, Text, Article, and PDF — to identify the most effective content delivery method by views and engagement.
* Regional Performance: Engagement was broken down by region to identify which markets are most active and where content resonates most strongly with audiences.
* Time and Day Analysis: Engagement was analysed by day of the week and time slot (8am–10am, 11am–1pm, 2pm–4pm, 5pm–7pm) to uncover peak posting windows across the dataset.
* Organic vs. Sponsored Content: The performance of organic posts (4,646) was compared against sponsored content (954) across all regions to evaluate the return on paid content investment.

## Dashboard
<img width="1392" height="820" alt="Screenshot (190)" src="https://github.com/user-attachments/assets/9aea9d6b-94ef-4f93-ad17-d51f50b9f85d" />

## Key Insights
* YouTube generated the highest total engagement at 151,399,907, closely followed by TikTok (146,646,344) and Instagram (134,738,386)
* LinkedIn and Facebook were the lowest-performing platforms with 44,731,424 and 35,701,985 engagements respectively
* YouTube also dominated in video views and live stream metrics, reinforcing its position as the top platform for long-form and video content
* Educational content drove the highest engagement at 238,044,553, closely followed by Product Promotion at 223,339,503
* Event/Webinar content had the lowest engagement at 30,586,034, suggesting it appeals to a more niche audience segment
* Customer Story content generated 72,692,576 engagements — a strong category for building trust and relatability
* Video posts dominated views with 3,641,141,686 views, far exceeding all other formats
* Live Stream content accumulated 349,751,811 views, making it the second most-viewed format
* Image posts led in non-video reach with 357,758,451 views
* PDF and Article formats had the lowest view counts, suggesting limited organic reach on social platforms
* USA generated the highest total engagement at 90,559,635, followed by Japan (82,781,768) and Brazil (82,642,904)
* Germany had the lowest regional engagement at 71,288,254, though still substantial in absolute terms
* Across all regions, sponsored content consistently outperformed organic on a per-post basis, with the USA leading in both organic and sponsored performance
* The 2pm–4pm time slot generated the highest total engagement at 193,187,693, closely followed by 11am–1pm (192,102,605)
* Wednesday was the strongest performing day with 100,405,596 engagements, followed by Saturday (97,835,985)
* Tuesday was the weakest day at 87,456,626 engagements
* The 8am–10am and 5pm–7pm slots were consistently the lowest performing across all days
* ProductDemo drove the highest impressions at 1,963,906,537, making it the most impactful hashtag in the dataset
* #CustomerStory followed with 1,212,705,940 impressions, reinforcing the value of storytelling content
* #FeatureHighlight had the lowest impressions at 198,290,143
* Of the 5,600 posts, 4,646 were organic (83%) and 954 were sponsored (17%)
* Despite the lower volume, sponsored content delivered strong engagement, particularly in the USA and UK
* Medium engagement was the most common outcome with 3,110 posts (55.5%)
* High engagement posts accounted for 1,320 (23.6%) and Low engagement for 1,170 (20.9%)

## Recommendations
* Prioritise YouTube and TikTok for video content — Both platforms lead in engagement and video views. Increasing the volume and quality of video content on these platforms should be a core content strategy priority.
* Double down on Educational and Product Promotion content — These two categories consistently drive the highest engagement. Content calendars should allocate the majority of posts to these categories.
* Post during the 11am–1pm and 2pm–4pm windows — These time slots consistently generate the highest engagement across all days. Scheduling posts within these windows maximises the likelihood of reaching active audiences.
* Target Wednesdays and Saturdays for high-priority content — These days deliver the strongest overall engagement and are ideal for launching campaigns, product announcements, or high-value content.
* Leverage #ProductDemo and #CustomerStory hashtags — These hashtags drove the highest impressions and should be incorporated into content planning for maximum organic reach.
* Expand USA and Japan market strategy — As the top two performing regions, these markets warrant increased content investment, tailored messaging, and potentially higher sponsored spend.
* Review LinkedIn and Facebook strategy — Both platforms significantly underperform compared to other channels. The content format, posting frequency, or audience targeting strategy on these platforms may need to be revisited.
* Increase Live Stream content — With 549,313,009 live stream views, live content generates significant audience interest. Brands should consider incorporating regular live sessions into their content mix, particularly for events and product launches.

## Limitations
* No demographic breakdown — The dataset does not include audience age, gender, or interest data, limiting the ability to analyse which audience segments are most engaged
* No cost data for sponsored posts — Without knowing the budget behind sponsored content, it is not possible to calculate ROI or cost per engagement for paid campaigns
* Platform algorithm changes not accounted for — Social media algorithms evolve frequently and can significantly affect reach and engagement, factors not captured in the dataset
* Hashtag data incomplete — Not all posts had a Main_Hashtag recorded, which may underrepresent the full impact of hashtag-driven reach
* Click data missing for many posts — The Clicks and Click_Through_Rate fields contained significant blank entries, limiting the depth of conversion and action-based analysis

## Conclusion
This analysis of 5,600 social media posts across six platforms and eight global regions revealed clear patterns in what drives content performance. YouTube and TikTok lead in engagement, video content dominates all other formats by a wide margin, and the 11am–4pm window on Wednesdays and Saturdays consistently delivers peak audience interaction. Educational and Product Promotion content are the highest-performing categories, while #ProductDemo and #CustomerStory hashtags generate the most impressive reach.

These insights provide a data-driven foundation for social media managers, content strategists, and marketing teams to make smarter decisions around platform investment, content planning, posting schedules, and audience targeting — ultimately improving social media performance and return on content investment.

## Project Files
[View main Excel workbook](./Social_Media_Content_Analysis.xlsx)

The Excel workbook contains:
* The raw dataset
* The analysis sheet
* The dashboard

## Contact Information
* Email: aladeloyeesther616@gmail.com
* LinkedIn: https://linkedin.com/in/estheraderonke
