# JavaScript

## Convert ISO Date to Date
[Convert ISO Date to Date Format yyyy-mm-dd format in javascript](https://stackoverflow.com/questions/25159330/convert-iso-date-to-date-format-yyyy-mm-dd-format-in-javascript)
```
   date = new Date('2013-03-10T02:00:00Z');
   date.getFullYear()+'-' + (date.getMonth()+1) + '-'+date.getDate();//prints expected format.
```