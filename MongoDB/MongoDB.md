# MongoDB

## Convert from text to Date type
[How do I convert a property in MongoDB from text to date type?](https://stackoverflow.com/questions/2900674/how-do-i-convert-a-property-in-mongodb-from-text-to-date-type)
```
   db.ClockTime.find().forEach(function(doc) {
     doc.ClockInTime=new Date(doc.ClockInTime);
     db.ClockTime.save(doc); 
   })
```

## Distinct Days, Months, Years
[Get distinct ISO dates by days, months, year](https://stackoverflow.com/questions/33109897/get-distinct-iso-dates-by-days-months-year)
```
   db.mycollection.aggregate([
     { "$project": { 
       "year": { "$year": "$date" }, 
       "month": { "$month": "$date" } 
       }
	 },
	 { "$group": { 
         "_id": null, 
         "distinctDate": { "$addToSet": { "year": "$year", "month": "$month" }}
       }
	 }
   ])
```

## Sorting Aggregation $addToSet
[Sorting aggregation addToSet result](https://stackoverflow.com/questions/21967233/sorting-aggregation-addtoset-result)
"Sets are considered to be unordered..."
```
   db.collection.aggregate([

     // Initial unwind
     {"$unwind": "$array"},

     // Do your $addToSet part
     {"$group": {"_id": null, "array": {"$addToSet": "$array" }}},

     // Unwind it again
     {"$unwind": "$array"},

     // Sort how you want to
     {"$sort": { "array": 1} },

     // Use $push for a regular array
     {"$group": { "_id": null, "array": {"$push": "$array" }}}

   ])
```