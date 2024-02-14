## Tableau Handbook

### Question
* How to display the **header** for a field that is being used only on the **Text** or **Label** card?
* How to name an **aggregated** column in Tableau?
#### Answer
## Additional resources - [resource](https://youtu.be/qgezLad4OnU)
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

