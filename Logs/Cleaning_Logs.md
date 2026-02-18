# Data Cleaning

## Columns Removed
- detailed_description, about_the_game, short_description, header_image, website, support_url, support_email
- reviews, metacritic_url, notes, screenshots, movies, user_score, score_rank, tags

## Type Conversions
- release_date to Date
- age to Number
- price to Currency
- metacritic_score to Number
- achievements to Number
- recommendations to Number
- positive to Number
- negative to Number
- average_playtime_forever to Number
- average_playtime_2weeks to Number
- median_playtime_forever to Number
- median_playtime_2weeks to Number
- discount to Percent
- peak_ccu to Number
- pct_pos_total to Number
- num_reviews_total to Number
- pct_pos_recent to Number
- num_reviews_recent to Number
- Windows, Mac, Linux to Boolean

## Array and Text Processing
- Counted supported_languages
- Counted full_audio_languages
- Split packages into main_packages count and sub_items count
- Converted developers array items to text
- Converted publishers array items to text
- Counted categories
- Counted genres
- Average of estimated_owners

## Title Standardization
- Removed "_" from titles
- Capitalized first letter of titles

# Data Analysis

## Analysis – Derived Columns

- Added Total Reviews (positive + negative) to represent overall review volume and sentiment credibility
- Added Weighted Sentiment (pct_pos_total × ln(total_reviews + 1)) to adjust sentiment by review volume and reduce low-sample bias
- Added Pricing Type (Free-to-Play / Paid) to classify games by monetization model
- Added Platform Count (Windows + Mac + Linux) to measure operating system accessibility
- Added Popularity Tier (Blockbuster / Hit / Mid / Niche) based on peak CCU thresholds for market segmentation
- Added Discount Impact (discount × peak_ccu) to estimate the relationship between discounting and player activity

## Analysis – KPIs

- Added Average Weighted Sentiment to summarize overall user sentiment adjusted for review volume
- Added Average Review Volume per Game to represent typical user engagement per title
- Added Sum Total Reviews to capture the overall scale of user feedback on the platform
- Added Average Peak CCU to measure average concurrent player activity and short-term popularity
- Added Popularity Tier Shares (Blockbuster, Hit, Mid, Niche) to analyze catalog distribution by popularity
- Added Review Concentration Ratios by popularity tier to assess engagement concentration across the catalog
- Added Free-to-Play Share to calculate the proportion of zero-priced games
- Added Paid Share to calculate the proportion of paid games
- Added Multi-Platform Game Share to measure catalog accessibility across operating systems
- Added Average Platform Count to evaluate average OS support per game
- Added Average Discount Impact as a proxy metric to explore pricing effects on activity
- Added Price Band to group games into interpretable pricing ranges
- Added DLC Band to group games by post-launch content depth
- Added Recommendation Band to group games by social proof intensity

## Analysis – Pivot Tables

- Added Average Peak CCU by Pricing Type to compare player reach between Free-to-Play and Paid games
- Added Average User Sentiment by Pricing Type to assess satisfaction differences across pricing models
- Added Review Volume by Popularity Tier to analyze how engagement is distributed across market segments
- Added Platform Accessibility by Popularity Tier to examine the link between OS support and popularity
- Added Average User Sentiment by Genre Count to evaluate how genre breadth relates to satisfaction
- Added Average Peak CCU by Genre Count to analyze the impact of genre diversity on player reach
- Added Popularity Tier Distribution by Pricing Type to understand pricing representation across tiers
- Added Average Peak CCU by Price Band to compare engagement across pricing ranges
- Added Average User Sentiment by Price Band to analyze sentiment variation by price level
- Added Average Peak CCU by DLC Band to assess the effect of content depth on engagement
- Added Average Peak CCU by Recommendation Band to evaluate the role of social proof in popularity

# Dashboard

- Added 5 main KPI cards for high-level performance tracking
- Added 4 charts focused on strategy by Pricing Type
- Added 3 charts focused on strategy by Popularity and Engagement
- Added 3 charts focused on strategy by Content Type
- Added 5 slicers based on key analytical metrics
- Updated color scheme to a darker theme aligned with the Steam desktop interface
- Added a pricing split pie chart to show catalog composition
- Enhanced slicer coverage with section-specific slicers
- Added additional high-impact KPIs for deeper insight
- Improved chart monotonicity by selecting more suitable chart types
- Added 3 navigation buttons to move between analysis sections
- Added explanatory notes to selected charts for clarity
- Ensured all key insights reflect a business decision-making perspective
- Updated charts within the Pricing Analysis section
- Applied 3D styling to selected charts for improved visual appeal
- Added dedicated slicers for KPI cards
- Verified full slicer functionality across the dashboard