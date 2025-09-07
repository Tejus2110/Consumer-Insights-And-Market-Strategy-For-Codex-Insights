# Energy Drink Market Analysis – CodeX

## Project Overview  

This repository presents a detailed data analysis project focused on understanding the energy drink market in India, specifically for the launch of **CodeX**, a new energy drink brand. The study is based on a large-scale survey of **10,000 respondents across 10 Indian cities**, capturing consumer demographics, perceptions, consumption habits, and brand preferences.  

The objective of this project was to provide the marketing and product development teams with actionable insights by:  

1. Exploring **who consumes energy drinks**, how frequently, and under what circumstances.  
2. Identifying the **motivations behind consumption** and the main barriers preventing trial.  
3. Examining **brand awareness, reputation, and positioning** in the competitive landscape.  
4. Understanding **health perceptions** and consumer demand for natural or organic alternatives.  
5. Recommending **pricing strategies, packaging preferences, and marketing channels** for CodeX.  

The analysis employed **statistical data analysis techniques**, including:  
- Univariate and bivariate analysis  
- Chi-square tests for association  
- One-way ANOVA with post-hoc testing  
- Cramer’s V for effect size evaluation  
- Visualization of results through charts and plots  

The final outcome is a **comprehensive strategic recommendation framework** for CodeX’s entry into the Indian market.  

---

## Repository Structure  

This repository contains the following files:  

| File | Description |
|------|-------------|
| **Final_Code_File.ipynb** | Jupyter Notebook containing the complete analysis workflow. This file includes data preprocessing, exploratory data analysis, statistical testing, and visualization. |
| **dim_respondents.csv** | A dimension table providing demographic details of respondents, including age group, gender, and associated city. |
| **dim_cities.csv** | A dimension table mapping each city to its name and tier classification. |
| **fact_survey_responses.csv** | A fact table containing the actual survey responses, such as consumption frequency, brand awareness, perceptions, and purchase behavior. |
| **Metadata.txt** | Documentation describing all dataset columns and their meanings, covering respondent demographics, city information, and survey response variables. |
| **Survey_Questions_and_Response_Options.pdf** | The survey instrument used to collect responses, including all questions and the range of response options provided to participants. |
| **raw_insights.txt** | Preliminary univariate and bivariate insights generated during analysis. Includes detailed statistical test results, such as chi-square outcomes and ANOVA results. |
| **Primary_Secondary_Insights.pdf** | Draft insights and guiding questions for both primary survey analysis and secondary market research. Provides an initial framework for deriving business recommendations. |
| **Comprehensive_Analysis_FULL_VERSION.pdf** | The final consolidated report synthesizing all findings. This report includes statistical validation, detailed segmentation insights, and an executive summary with actionable recommendations. |
| **Visual Assets (PNG files)** | Supporting charts and plots produced during the analysis to visualize key results. |

---

## Dataset Description  

The dataset is organized in a star-schema-like format, consisting of three main tables:  

### 1. `dim_respondents`  
Contains demographic attributes of survey participants:  
- **Respondent_ID**: Unique identifier for each respondent  
- **Name**: Name of the respondent  
- **Age_Group**: Categorized into groups (15–18, 19–30, 31–45, 46–65, 65+)  
- **Gender**: Male, Female, or Non-binary  
- **City_ID**: Links the respondent to their city in `dim_cities`  

### 2. `dim_cities`  
Contains city-level attributes:  
- **City_ID**: Unique city identifier  
- **City**: City name (Delhi, Mumbai, Bangalore, Chennai, Kolkata, Hyderabad, Ahmedabad, Pune, Jaipur, Lucknow)  
- **Tier**: Classification of city into Tier 1 or Tier 2  

### 3. `fact_survey_responses`  
Captures the survey responses for each participant. Key fields include:  
- **Consume_frequency**: How often energy drinks are consumed (Daily, Weekly, Monthly, Rarely)  
- **Consume_time**: Typical consumption times (Before exercise, During study/work, etc.)  
- **Consume_reason**: Motivations for consumption (Energy, Focus, Combat fatigue, Sports performance)  
- **Heard_before**: Whether respondents had heard of CodeX before the survey  
- **Brand_perception**: Perception of CodeX’s brand identity  
- **General_perception**: General views about energy drinks (Healthy, Effective, Dangerous, Not sure)  
- **Tried_before**: Whether respondents had tried CodeX before  
- **Taste_experience**: Rating of taste and overall experience (1–5 scale)  
- **Reasons_preventing_trying**: Barriers such as availability, health concerns, or unfamiliarity  
- **Current_brands**: Competing brands consumed (Cola-Coka, Bepsi, Gangster, etc.)  
- **Reasons_for_choosing_brands**: Drivers of brand choice (Reputation, Taste, Availability, Effectiveness)  
- **Improvements_desired**: Desired product improvements (Reduced sugar, More flavors, Natural ingredients)  
- **Ingredients_expected**: Key ingredients expected in an energy drink (Caffeine, Vitamins, Sugar, Guarana)  
- **Health_concerns**: Whether respondents are concerned about health effects  
- **Interest_in_natural_or_organic**: Willingness to try natural or organic alternatives  
- **Marketing_channels**: Channels where respondents encounter advertisements (TV, Online, Print, Billboards)  
- **Packaging_preference**: Packaging choices (Cans, Bottles, Eco-friendly, Collectibles)  
- **Limited_edition_packaging**: Interest in limited edition designs  
- **Price_range**: Reasonable price points for energy drinks  
- **Purchase_location**: Where respondents usually buy energy drinks (Supermarkets, Online, Gyms, etc.)  
- **Typical_consumption_situations**: Common scenarios of consumption (Sports, Study, Social events, Commuting)  

---

## Key Findings from the Comprehensive Analysis  

### 1. Demographics  
- The majority of respondents were **19–30 years old (55%)** and **male (60%)**.  
- Frequency of consumption is not significantly different across age or gender, suggesting broad, uniform consumption patterns.  
- The most important **target segment** for CodeX is young adults in Tier 1 cities.  

### 2. Geographic Insights  
- **Bangalore and Chennai**: Highest rates of frequent consumption.  
- **Delhi and Mumbai**: Highest brand awareness but limited trial, highlighting a conversion problem.  
- **Tier 2 cities (e.g., Pune, Ahmedabad, Jaipur)**: Negative brand perceptions and availability issues require urgent attention.  

### 3. Consumption Patterns  
- The most common consumption frequency is **2–3 times per week (35%)**.  
- Primary consumption contexts: **sports/exercise (45%)** and **studying/working late (32%)**.  
- Motivations: **energy and focus (36%)** and **combat fatigue (24%)**.  

### 4. Health Perceptions and Ingredients  
- **60% of respondents** express health concerns about energy drinks.  
- **50% indicate interest in natural or organic alternatives**.  
- Desired improvements: Reduced sugar (30%), natural ingredients (25%), wider range of flavors (20%).  

### 5. Packaging Preferences  
- Preferred formats: **compact cans (40%)** and **innovative bottles (30%)**.  
- Limited-edition packaging divides opinion, with nearly equal interest and disinterest.  

### 6. Brand Awareness and Perception  
- **55% have heard of CodeX**, but only **20% have tried it**.  
- Overall perception is neutral, though **negative sentiment is concentrated in Tier 2 cities**.  
- Taste ratings are average (~3.5/5), indicating potential for product improvement.  

### 7. Competitive Landscape  
- Market leaders are **Cola-Coka (25%), Bepsi (21%), and Gangster (19%)**.  
- Consumers prioritize **brand reputation (27%)**, **taste (20%)**, and **availability (19%)** when choosing brands.  
- CodeX must invest heavily in **building its reputation** and improving product taste to compete effectively.  

### 8. Marketing Channels  
- **Online advertising (40%)** is the most effective channel, especially for younger audiences.  
- **TV commercials (27%)** have broad reach but low trial conversion.  
- Male respondents are more responsive to outdoor advertising, while female respondents lean toward print and influencer-driven campaigns.  

### 9. Pricing and Purchase Behavior  
- Most consumers expect energy drinks to be priced between **₹50–99**, with older professionals willing to accept **₹100–150**.  
- **Supermarkets (45%)** and **online retailers (26%)** are the most common purchase locations.  

---

## Strategic Recommendations  

Based on the findings of this study, several strategies are recommended for CodeX:  

1. **Target Audience**  
   Focus marketing on **young urban adults (15–30 years old)**, particularly those living in Tier 1 cities. This group represents the largest and most consistent consumer base, and their openness to energy drinks positions them as the primary market segment for CodeX.  

2. **Product Positioning**  
   Position CodeX as a **better-for-you performance drink**. Emphasize caffeine and vitamins for energy and focus, while highlighting reduced sugar and natural ingredients to appeal to health-conscious consumers. This positioning will differentiate CodeX in a market where health concerns are a major deterrent.  

3. **Pricing Strategy**  
   Offer a **core product priced between ₹50–99**, which aligns with the expectations of younger consumers and ensures competitiveness against established brands. Introduce a **premium variant at ₹100–150** aimed at working professionals who are willing to pay more for added health benefits, improved flavors, or enhanced packaging. This dual pricing approach ensures broader market coverage.  

4. **Distribution Strategy**  
   Strengthen presence in **supermarkets and online retail platforms**, as these are the dominant purchase locations. Special attention should be given to **Tier 2 cities**, where availability is a major barrier. Expanding distribution networks and ensuring consistent stock in these regions will directly address consumer frustrations and improve trial rates.  

5. **Marketing Strategy**  
   - Invest in **digital and social media campaigns**, as younger demographics (15–30) overwhelmingly encounter energy drink advertisements online. This should include targeted advertising across social platforms, student communities, and fitness-related content.  
   - **Revise the TV advertising approach** for older audiences. While TV ads reach a wide base, their conversion rates are low. Tailored messaging emphasizing safety, reliability, and health benefits may increase their effectiveness.  
   - Consider appointing a **sports or fitness ambassador** to reinforce the product’s reputation and appeal to performance-oriented consumers. This would also strengthen the brand’s competitive positioning against market leaders.  

6. **Product Development**  
   Improve the **taste and flavor variety** of CodeX, as competitor brands are often chosen based on taste and brand reputation. Alongside taste, focus on **reduced sugar content and natural ingredients** to align with consumer demands for healthier alternatives. Seasonal or limited-edition flavors can also be introduced to create novelty and excitement around the brand.  

7. **Packaging Strategy**  
   Launch primarily in **compact cans and innovative bottles**, which are the most preferred packaging formats. Occasionally introduce **limited-edition packaging** as a marketing tool to create short-term excitement and encourage repeat purchases, but keep it as a supplementary rather than core strategy.  

---

## How to Use This Repository  

1. Open the Jupyter Notebook `Final_Code_File.ipynb` to follow the complete analysis process.  
2. Review `Metadata.txt` for detailed dataset schema and definitions.  
3. Consult `raw_insights.txt` for statistical test results and initial findings.  
4. Refer to `Comprehensive_Analysis_FULL_VERSION.pdf` for the final consolidated report and recommendations.  
5. Examine the survey documentation (`Survey_Questions_and_Response_Options.pdf`) to understand the question design and response framework.  
