# MongoDB

## Convert from text to Date type
[How do I convert a property in MongoDB from text to date type?](https://stackoverflow.com/questions/2900674/how-do-i-convert-a-property-in-mongodb-from-text-to-date-type)
```
   db.ClockTime.find().forEach(function(doc) {
     doc.ClockInTime=new Date(doc.ClockInTime);
     db.ClockTime.save(doc); 
   })
```