# real time currency converter
![currency](https://user-images.githubusercontent.com/69091817/131383366-691fb343-46ad-4adf-803d-d49eaf1fcc7e.png)

In this project, we create a function that converts a given amount of a source currency into its equivalent in a target currency.
The function uses the **US Dollar (USD)** as base currency, that is the exchange rates are given with respect to USD. 

|currency | rate (1 USD = rate * currency)|
|:-------:|:------------------------------: |
| English Pound (GBP)    | 0.727      |
| Indian Rupee (INR) | 73.66            |
| Central African CFA Franc (XAF) | 556.38 |
<br>
Table 1: Example conversion rates from Mon, 30 Aug 2021 00:02:31 UTC update
<br>
The conversion between two currencies (input_curr and output_curr) each different from USD is made as follows: <br>
**(amount / rate_input_curr) x rate_output_curr**

The function firstly checks the internet connection. If the result is True, the real time conversion rates are used and the 
stored old rates are updated , otherwise the old rate is used.


## Required packages
- requests
- json
- socket
