***

It consists in grouping tables as:

- **Fact Table:** Has ***business events*** and its ***metrics***
- **Dimension Table:** Has ***detailed context*** about the *metrics*.

*Fact tables* are characterized because they provide ***quantitative*** data, while *dimension tables* focus on ***qualitative*** data.

Its theoretical evolution is the ***Snowflake Schema***, in which *dimension tables* can also be *fact tables* simultaneously. 

It prioritizes **easier queries** at the cost of **storage**.

***

