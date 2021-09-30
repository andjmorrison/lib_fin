# Example Library Financial Analysis

This repository showcases some commonplace analyses for library acquisitions data, including:

* [x] yearly ggregations per internal fund code and vendor
* [x] LC subject area totals

Pandas and regular expressions prove *highly* useful when performing any analysis of bibliometric datasets. For example, using 

``` df[col].str.extract(r'([^\|a][A-Z]{0,4})') ``` 

to strip out the LC subject headings from a column of ```MARC 090``` fields is much simpler than iterating through each row of the data and wrangling strings in a more manual fashion. In this capacity, even a dataset containing expenditures and corresponding call number *only* can be useful for performing analysis.

---

Because this financial data are internal, no ```CSV``` files have been provided.