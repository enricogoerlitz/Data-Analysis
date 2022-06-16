# EDA Project: Bank loan data analysis

## General

Author: Enrico Goerlitz <br/>
Initial Date: 16.06.2022

## Description

This project is an EDA of the loan data of a bank. <br>
We want to find out, which and how features got an impact on the pay back of the loans. <br>
Therefor, we will aks us the following questions (next section) and proceed as follows: <br>

-   describe process...

In the end we want to say, which kind features and corresponding data got an positive and which got an negative effect on the pay back. So that we focus on them when granting the loan.

## Data questions

<ol>
    <li>What are good loan pay back data? (We need to define this!)</li>
    <li>Which features got an impact on the loan pay back?</li>
    <li>Which features and there corresponding data got an positive and which got an negative effect on the loan pay back?</li>
    <li>How does the best and the worst loan data looks like?</li>
</ol>

## Data cleaning & preprocessing

(!!! - EDIT THIS - !!!)

-   rename `issue_d` to `issue_month`
-   split the columns `issue_month` into month and year (year as new column and month as number (1 - 12))
-   interpolate missing values of the `issue_month` with the mean or mode
-   interpolate `loan_amnt` (therefor, take a look at the funded_amnt, loan_status, total_pymnt, term and installment)
-   interpolate `loan_status`
-   interpolate `funded_amnt` (therefor, take a look at the loan_amnt, loan_status, total_pymnt, term and installment)
-   remove "months" from `term` so that the columns is full of integers
-   interpolate `term` (therefor, take a look at the other columns)
-   interpolate `int_rate` (therefor, take a look at the other columns)
-   interpolate `installment` (therefor, take a look at the other columns)
-   interpolate `grade` (therefor, take a look at the `sub_garde` column)
-   interpolate `sub_grade` (therefor, take a look at the `garde` column)
-   interpolate `verification_status` (therefor, take a look at the other columns or/and expect the worst)
-   drop the `url` column
-   rename `addr_state` to `state`
-   clean the `state` column
-   add the column `int_rate_total` (int_rate / installment)
-   add the column `int_rate_percentage` (`int_rate_total` / `loan_amnt`)
-   add the column `loan_class` (classify the `loan_amnt` to {high_loan, normal_loan (q=2/3), low_loan (q=1/3)})
-   add the column `quarter` {Q1, Q2, Q3, Q4}

In general, at missing values, we will proceed very conservative and expect the worst.

## Used technologies

Python <br>
NumPy <br>
Pandas <br>
Matplotlib <br>
Seaborn <br>

## Used resources

https://unsplash.com/ <br>
https://unsplash.com/photos/NpTbVOkkom8 <br>
https://stackoverflow.com/ <br>

## Copyright

All licenses in this repository are copyrighted by their respective authors. <br>
Everything else is released under CC0. See `LICENSE` for details.
