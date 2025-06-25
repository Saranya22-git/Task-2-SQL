# **Data Insertion and Handling Nulls**📗
Here we learn about **Insert**, **Update** and **Delete** statements.
# 🔐Inserting
### -The SQL INSERT INTO statement is one of the most essential commands for adding new data into a database table.
### -The INSERT INTO statement is used to insert new records in a table.

## Inserting Data into All Columns: 
  This method is used when we want to insert data into all columns of a table without specifying column names. 
### **Syntax**: 
               INSERT INTO table_name
               VALUES (value 1, value 2, value 3);
### **For Example**: 
               INSERT INTO student_details
               VALUES (1,"Rama","Krishna","2003-11-11","Male","English",2000);
               
## Inserting Data multiple rows at once:
   This method is used to insert data in a single query.
### **Syntax**:
              INSERT INTO table_name
              VALUES (value 1, value 2, value 3....),
                     (value 1, value 2, value 3....);
### **For Example**:
              INSERT INTO student_details
              VALUES (2,"Sai","Ram","2004-12-02","Male","Physics",3000),
	                 (3,"Priyanka","Chowdary","2005-09-10","Female","Maths",3000),
                     (4,"Satya","Sri","1990-06-13","Female","Computer",2500),
                     (5,"Adnan","Shafi","2005-05-26","Male","Science",3000);
                     
## Inserting Data Into Specific Columns
  This method is used only when we want to insert data only specific column names.
### **Syntax**:
              INSERT INTO table_name (column_name1, column_name2)
              VALUES (value 1, value 2, value 3);
### **For Example**:
              INSERT INTO student_details (stu_id,first_name,course,payment)
              VALUES(6,"saranya","Chemistry",2500);

# 📑Updating
### -In SQL, the UPDATE statement is used to modify existing records in a table.
### **Syntax**: 
             UPDATE table_name
             SET column_name=value
             WHERE condition;
### **For Example**:
             UPDATE student_details
             SET stu_gender="Female"
             WHERE stu_id=6;
             
## Updating Data in Multiple columns
   This method is used to update multiple columns at a time.
### **Syntax**: 
             UPDATE table_name
             SET column1=value 1, column2=value2
             WHERE condition;
### **For Example**:
             UPDATE student_details
             SET last_name="Jain",Course="Chemistry"
             WHERE stu_id=3;
             
# 🗑️Deleting Statement
### -In SQL,the DELETE statement is used to delete rows in a table and it also removes the entire table.
### **Syntax**:
            DELETE FROM table_name
            WHERE condition;
### **For Example**:
            DELETE FROM student_details
            WHERE stu_id=1;
            
