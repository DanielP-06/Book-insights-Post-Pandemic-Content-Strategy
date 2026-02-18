# Book-insights-Post-Pandemic-Content-Strategy
Post-pandemic digital reading market analysis for startups. Using SQL and Python, we identified key authors (J.K. Rowling), publishers (Penguin Books), and active user patterns to optimize content strategy. Proposals include focusing on modern literature, gamifying reviews, and implementing quality filters.

# Digital Reading Content Strategy - Post-Pandemic Analysis

## Project Overview
This project provides a comprehensive data-driven analysis of the digital reading market post-pandemic, focusing on identifying key content trends, influential authors, and publishers, and understanding active user behavior. The insights derived are crucial for digital reading content startups to refine their value proposition and strategy in a saturated market.

## Problem Statement
The digital reading market is highly saturated following a surge in reading activity during the pandemic lockdowns. Startups offering digital reading content need to understand which types of authors, publishers, and books generate the most interest and engagement to develop a compelling value proposition.

## Objectives
1.  **Volume Audit:** Quantify the supply of modern content (books published after January 1, 2000).
2.  **Quality & Relevance:** Identify the most relevant authors and publishers on the platform, filtering out low-quality content or brochures shorter than 50 pages.
3.  **User Analysis:** Understand the behavior of the most active users to identify review patterns and engagement drivers.

## Methodology
This project leverages SQL queries to extract and analyze data from a PostgreSQL database containing information about books, authors, publishers, ratings, and reviews. Pandas is used for data manipulation and analysis, and Matplotlib along with Seaborn for data visualization.

Key analytical steps included:
*   **Database Connection:** Establishing a connection to the PostgreSQL database using `SQLAlchemy`.
*   **Preliminary Exploration:** Inspecting tables (`books`, `authors`, `publishers`, `ratings`, `reviews`) to understand data structure.
*   **Content Volume Analysis:** Counting modern books based on publication date.
*   **Book Quality Assessment:** Calculating average ratings and review counts per book.
*   **Publisher Impact:** Identifying publishers with the highest number of quality books (over 50 pages).
*   **Author Relevance:** Determining authors with the highest average ratings for books with significant user engagement (at least 50 ratings).
*   **User Engagement Analysis:** Calculating the average number of text reviews from highly active users (those who rated over 50 books).
*   **Data Visualization:** Creating bar plots to visualize top authors by average rating.

## Key Findings
*   **Modern Content Volume:** 819 books were published after January 1, 2000, indicating a significant modern content base.
*   **Leading Publisher:** Penguin Books is the top publisher with 42 quality titles (over 50 pages), highlighting its strong market presence in substantial content.
*   **Top-Rated Author:** J.K. Rowling/Mary GrandPré leads with the highest average rating (4.2871) among books with high user attraction (50+ ratings), signifying strong audience approval.
*   **Diversified Quality Authors:** Authors like Markus Zusak and J.R.R. Tolkien also show high-quality retention, suggesting opportunities for content diversification.
*   **Active User Behavior:** Users who rated over 50 books write an average of 24.33 text reviews, demonstrating their high engagement and influence as content curators.

## Recommendations
*   **Focus on Modern Books:** Target a young-adult audience interested in contemporary literature, aligning marketing efforts with books published post-2000.
*   **Strengthen Publisher Alliances:** Deepen partnerships with leading publishers like Penguin Books to secure a consistent supply of high-quality, long-form content.
*   **Gamify Reviews:** Implement a badge system or similar motivational incentives for active users who exceed 20 reviews to encourage continued text review contributions, leveraging their influence to build trust and guide new readers.
*   **Permanent Quality Filter:** Introduce a permanent quality filter in the application's search functionality, such as a minimum page count or rating threshold, to ensure users consistently discover high-value content and prevent low-quality items from distorting rankings.
