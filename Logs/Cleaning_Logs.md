# Data Cleaning Logs

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

