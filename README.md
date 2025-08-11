# Fact-Modeling-Players-Behavior

Turning to denormalized game details table to have all the dimensions and facts for player behavior analysis. 

Joins game_details with games to enrich records with game date, season, and home team info.
Deduplicates entries by game_id, team_id, and player_id using row numbering, keeping the earliest game record.
Filters data for a specific game date (2016-10-04).
Data Inserted


Dimensions:
Game date (dim_game_date)
Season (dim_season)
Team ID (dim_team_id)
Player ID and name (dim_player_id, dim_player_name)
Starting position (dim_start_position)
Player status flags:
Did Not Play (dim_did_not_play)
Did Not Dress (dim_did_not_dress)
Not With Team (dim_not_with_team)


Measures:
Minutes played converted from "MM:SS" to decimal hours (m_minutes)
Field goals, three-pointers, free throws (made and attempted)
Rebounds (offensive, defensive, total)
Assists, steals, blocks, turnovers, fouls
Points scored and plus-minus metric

<img width="1211" height="454" alt="Screenshot 2025-08-11 at 12 29 19 PM" src="https://github.com/user-attachments/assets/f6b71f29-18a7-4a5c-97fd-5ba3361cd35f" />
