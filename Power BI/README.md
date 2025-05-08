# 📱 App Analytics with Power BI

This Power BI project analyzes app data to uncover trends in app characteristics, user reviews, and developer responsiveness. The project is divided into three parts: exploring the app landscape, analyzing user reviews, and evaluating developer performance based on review interactions.

---

## 📊 Part 1: App Landscape

In this section, I created a dashboard titled **App Landscape** to explore high-level statistics about apps:

- **KPI Card** displaying the total number of unique apps.
- **Line Chart** showing the total number of reviews over time using the `lastmod` date.
- **Scatterplot** analyzing the relationship between review count and average rating, supplemented with an interpretation textbox.

---

## 📝 Part 2: Reviews

A new report page named **Reviews** was created to analyze the quality and responsiveness of reviews:

- Created a new DAX column `helpful_reviews` to weight ratings by helpfulness using the formula:  
  `helpful_reviews = rating * (1 + helpful_count)`.  
  Displayed the **average helpful review score** using a Card visualization.
- Created another DAX column `developer_answered` to flag whether a developer responded to a review.
- Built a **scatterplot** comparing average rating vs. developer responsiveness (0 or 1) using the `developer_answered` flag.

---

## 🧩 Part 3: App Reviews

The final section, titled **App Reviews**, focused on integrating and analyzing developer performance:

- Established a **many-to-one relationship** between the `Reviews` table (`app_id`) and the `Apps` table (`id`).
- Created a **bar chart** showing the sum of ratings per developer, then refined it by plotting **average helpful review scores** to correct for misleading totals.
- Developed a chart to evaluate **developer responsiveness**, filtering to only include apps with more than 500 reviews, and used the `developer_answered` column to show which developers are most engaged.

---

This project delivers insights into how app developers can enhance user satisfaction by understanding review patterns and engagement metrics.
