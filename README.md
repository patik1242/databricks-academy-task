**WHY THIS DATASET?**
The diversity of columns describing animals' features can help better understand admitted animals, for example whether more females or males are admitted, 
whether animals are more often surrender by owners or brought through public assistance and whether they are sterilized or non-sterilized 
(from few different columns we can extract so many information).

**WHY I CREATED THE NEW COLUMN `has_name`**
The `name` column contains missing values. That's why I created a new binary column `has_name` containing information whether an animal has a name at intake. 
This transformation can be useful because named animals could be lost, could return to owner or have higher chances of being adopted. After creating the column `has_name`, 
the name was removed. There was no need to drop rows with the missing value in `name` because we could lose potentially necessary information in the future analysis.

**CONCLUSIONS**
When it comes to the DataFrame, it was surprising that so much information could be extracted from only a few columns (sex, sterilization status, age group, day of week, month, hour). 
This information can be useful to the future analyze whether animals are admitted often during weekend or weekdays (or during which month, what holiday, season is it winter or spring?) 
from which areas animals are found or whether most animals are admitted in normal condition. 
From the SQL query I noticed that during weekend adult dogs were admitted to the shelter more often than young or senior. If I had more time, 
I could explore which breeds and colors are the most common, whether animals are more often stray or owner surrendered or in which month there are most intakes. 
I could also create better column of `age_group` because the age_group depends not only on days but also on the animal type. 
These kind of information could be helpful not only for analysis, but also for improving animal care in shelters through better awareness of admitted animals' features
