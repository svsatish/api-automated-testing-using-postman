## Library API:

#### Base URI:  

- UAT - https://rahulshettyacademy.com
- QA - http://216.10.245.166
 
1.	Add Book Complete URL - https://rahulshettyacademy.com/Library/Addbook.php

Method: POST

- note: aisle value should be number only. Isbn should be unique to insert. So provide random isbn which makes unique

Input Payload Json:
```json
{

"name":"Learn Appium Automation with Java",
"isbn":"bcd",
"aisle":"227",
"author":"John foe"
}
```

Output Json:
```json
{
   "Msg": "successfully added",
   "ID": "bcd227"
} 
```

 
2.	Get Book by author Resource : /Library/GetBook.php?AuthorName=somename

Method : GET
 
Output Json:

Output the array of Json object books with all below details 
```json 
[
{
Name : “bookname”,
Isbn :  “A2fdsf”,
Aisle : 32
}
]
```

3. Get Book by ID Resource: Library/GetBook.php?ID=3389

Method : GET 

Output Json:
```json
{
"book_name": "Selenium automation using Java",
"isbn": "a23hd738",
"aisle": "1223"
} 
```

4. Delete Book Resource :/Library/DeleteBook.php

Method : POST
 
Input Payload Json:
```json
{
"ID" : "a23h345122332"
} 
```

Output Response:
```json
{
msg : "book is successfully deleted"
}
```
