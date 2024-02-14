## Tableau Handbook

### Question
* How to display the **header** for a field that is being used only on the **Text** or **Label** card?
* How to name an **aggregated** column in Tableau?
#### Answer
## Additional resources - [Resource](https://youtu.be/qgezLad4OnU)
#### ****Option 1****

1.  Drag **Measure Names** from Dimensions to **Columns**.
2.  Drag **Measure Values** from Measures to  **Detail**.
3.  Right-click  **Measure Names**  on  **Columns** and then select **Filter**.
4.  Click  **None**  and then select the fields whose headers you want to display.
5.  Click **OK**.

#### ****Option 2****(*Preferred*)

1.  Drag  **Measure Names**  from Dimensions to **Columns**.
2.  Right-click the header of the column that needs a title. It will likely say  **No Measure Name**.
3.  Select  **Edit Alias**.
4.  Type the new title and then click  **OK**.

#### ****Option 3 (For only one measure)****

1.  Click  **Analysis**  >  **Create a new calculated field...**
2.  Name the calculated field "Title" and in the formula, add the name of the column that you wish to use in quotes. For example:
    
    "Sales"
    
3.  Drag the newly created field "Title" to  **Columns**.
4.  Right-click on the text "Title" and select  **Hide field labels for columns**.


### Question

* How to change the dimension header in crosstab without actually changing the Dimension Name in the data source?

  
![User-added image](https://kb.tableau.com/servlet/rtaImage?eid=ka06Q000000tfFk&feoid=00N60000002Wwyw&refid=0EM6Q0000027gsV)

#### **Environment**

-   Tableau Desktop

#### **Answer**

The ability to only change the dimension header in the view is not currently built into Tableau Desktop.  
  
Consider the workaround which achieves similar functionality.  
  
Please note that this method only applies to  [Dimensions](https://help.tableau.com/current/pro/desktop/en-us/datafields_typesandroles.htm) (Discrete or Continuous). When you are using Dates, Measures, or Attributes that are other than a Dimension, this workaround is not applicable.

##### **Follow the steps below:**

1. Double-click the dimension added to the [Rows/Columns] shelf.

![User-added image](https://kb.tableau.com/servlet/rtaImage?eid=ka06Q000000tfFk&feoid=00N60000002Wwyx&refid=0EM6Q0000027gsf)

2. Add "//Dimension Name" at the beginning.

![User-added image](https://kb.tableau.com/servlet/rtaImage?eid=ka06Q000000tfFk&feoid=00N60000002Wwyx&refid=0EM6Q0000027gsk)

3. Press "Shift + Enter" to add a new line character.

![User-added image](https://kb.tableau.com/servlet/rtaImage?eid=ka06Q000000tfFk&feoid=00N60000002Wwyx&refid=0EM6Q0000027gsp)  

Finally, the dimension header can be changed like in the below image.

![User-added image](https://kb.tableau.com/servlet/rtaImage?eid=ka06Q000000tfFk&feoid=00N60000002Wwyx&refid=0EM6Q0000027gsu)  
* The dimension in the [Rows/Columns] shelf has two lines like below and it will show the  **first line as the header**  and show  **the dimension in the second line.**  
---------------------  
//Dimension Name  
[Category]  
---------------------
