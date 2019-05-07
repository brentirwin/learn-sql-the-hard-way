1. If you got rid of the able person_pet and put that information right into person, it would imply that a person could only have one pet, but that multiple people could have the same pet.
2. Yes of course you can put more than one row into person_pet. You would record a crazy cat lady with 50 cats by putting the lady's ID in multiple rows, one for each of the cats' ID's.
3.
```sql
CREATE TABLE car (
  vin INTEGER PRIMARY KEY,
  make TEXT,
  model TEXT,
  color TEXT
);

CREATE TABLE person_car (
  person_id INTEGER,
  car_vin INTEGER
);
```
4. The first 4 data classes - null, integer, real, and text - are straightforward to any programmer. Blob is a binary chunk of anything. That makes sense. There are three different ways to store dates. Integer is a Unix timestamp. Text is in format "YYYY-MM-DD HH;MM;SS.sss". That's simple. Having a real number represent the number of days since some strange Abrahamic epoch doesn't make any sense, but I'm sure a use for it might come up sometime.
