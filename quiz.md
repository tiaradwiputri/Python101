# Introduction to Pandas

The following quiz set is created as an accompanying quiz for knowledge assessment purposes.

## Object Oriented Programming

1. The syntax used to access Python object's attributes such as methods and attributes is...
	- [ ] `.`  
	- [ ] `_`  
	- [ ] `self`  
	- [ ] `def`  

2. When you import `pandas` package to read a flat CSV files, you will access `read_csv` as one of its attribute with the following syntax: `pandas.read_csv()`. The `read_csv` is referred as a *method*, which can be accessed by calling it with double brackets `()`. The method, will need a parameter of `file_path`. Say you are storing your csv file named `data.csv` under a folder named `data` on your project folder. How would you pass the `file_path` parameter for the method?
	- [ ] `pandas.read_csv("data/data")`  
	- [ ] `pandas.read_csv("data.csv")`  
	- [ ] `pandas.read_csv("data/data.csv")`  
	- [ ] `pandas.read_csv("../data/data.csv")`  

3. The `data.csv` you loaded on previous question is then stored in an object called `my_data`. What tyoe of object is the data stored in?
	- [ ] Object  
	- [ ] pandas  
	- [ ] DataFrame  
	- [ ] List  

## Data Wrangling

4. The following are some of the technique you can use to subset your DataFrame, except...
	- [ ] `.iloc[]`  
	- [ ] `.loc[]`  
	- [ ] `.dtypes`  
	- [ ] `.select_dtypes()`  

5. Say you have 3 different numeric columns you need to modify. Each of the column have the unit in thousand, so to have the number stored correctly you want to have the 3 columns multiply by 1000. To apply a *nameless function* on the column you can use a *lambda* using `apply` method. Which of the following is the correct command to do so?
	- [ ] `data[['A','B', 'C']].apply(lambda x*1000)`  
	- [ ] `data[['A','B', 'C']].lambda(x*1000)`  
	- [ ] `data[['A','B', 'C']].apply(lambda x); def x: x*1000`  
	- [ ] `data[['A','B', 'C']].apply(lambda x: x*1000)`  

6. Other useful subsetting techniques known as conditional subsetting. This technique use a set of condition to filter our data frame. Say you would like to have a certain data frame that filter the following from your initial data: All column A need to be equal to 0 and Either column B or C need to have the value of: "AVAILABLE" or "IN STOCK". Which of the following will filter the data frame correctly?
 	- [ ] `data[data.A == 0 & data.B.isin(["AVAILABLE", "IN STOCK"] | data.C.isin(["AVAILABLE", "IN STOCK"])) ]`  
	- [ ] `data[(data.A == 0) & (data[['B',C]].isin(["AVAILABLE", "IN STOCK"]))]`  
	- [ ] `data[(data.A == 0) & (data.B.isin(["AVAILABLE", "IN STOCK"]) | data.C.isin(["AVAILABLE", "IN STOCK"])) ]`  
	- [ ] `data[(data.A == 0) & (data.B.isin(["AVAILABLE", "IN STOCK"])) & (data.C.isin(["AVAILABLE", "IN STOCK"])) ]`  
