# Swiggy_Case_Study
In this case study, I have used different concepts of intermediate and Advanced SQL like CTE's, Window Functions, Nested Subqueries and Joins to gain relevant insights from the data.

### Tables Structure
<table>
<tr><th>users</th><th>restaurants</th><th>orders</th><th>order_details</th><th>menu</th><th>food</th></tr>
<tr><td>

|user_id|
|--|
|name|
|email|
|password|
</td><td>

|r_id|
|--|
|r_name|
|cuisine|
|rating|
</td>
<td>

|order_id|
|--|
|user_id|
|r_id|
|amount|
|date|

</td>
<td>

|id|
|--|
|order_id|
|f_id|

</td>
<td>

|menu_id|
|--|
|f_id|
|r_id|
|price|

</td>
<td>

|f_id|
|--|
|f_name|
|type|

</td>
</tr> </table>

### SQL Analysis

**Q1. Find customers who have never ordered**<br>
**Ans.** Anupama and Rishabh
<br><br>
**Q2. Find average Price per dish**
| f_name | avg_price  | 
| :---:   | :-: |
| Chicken popcorn | 300 |
| Chicken Wings | 230 |
| Choco Lava Cake | 98.33 |
| Masala Dosa | 180 |
| Non Veg Pizza | 450 |
| Rava Idli | 120 |
| Rice Meal | 213.33 |
| Roti Meal | 140 |
| Schezwan Noodles | 220 |
| Veg Manchurian | 180 |
| Veg Pizza | 400 |

<br><br>
**Q3. Top restaurant in terms of number of orders for a given month**<br>
**Ans** Dosa Plaza

<br><br>
**Q4. Find restaurants with monthly sales greater than 700 for a July month**<br>
**Ans** dominos and kfc

<br><br>
**Q5. Find restaurants with max repeated customers**
| r_name | uniuqe_customers  | 
| :---:   | :-: |
| KFC | 2 |

<br><br>
**Q6. Month Over Month revenue growth of Swiggy**
| Month_num | Monthly_revenue_growth  | 
| :---:   | :-: |
| 5 | NULL |
| 6 | 32.78 |
| 7 | 50.46 |
<br>
The above values are in %ages with respect to previous month

<br><br>
**Q7. Find the most loyal customers for all restaurant**
| r_name | name  | 
| :---:   | :-: |
| Dosa Plaza | Ankit |
| kfc | Neha |
| box8 | Nitish |
| kfc | Vartika |

**There are more questions discussed in coding file but their ouptut varies with different inputs**
