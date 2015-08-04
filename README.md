# dates-mail-merge
How to get the right date format from an Access to Word mail merge in MS office


To get the date format you want, you can add a formatting picture switch as follows:

• select the mergefield;

• press Shift-F9 to expose the field coding. It should look something like {MERGEFIELD MyDate} where 'MyDate' is your mergefield's name;

• delete anything appearing after the mergefield's name and add '\@ "dd-MMM-yy"' to the field, as in {MERGEFIELD MyDate \@ "d MMMM yyyy"}. With this switch your date will come out as '2 August 2008'. Other possible date formatting switches include:

. \@ "dddd, d MMMM yyyy";

. \@ "ddd, d MMMM yyyy";

. \@ "d MMM yyyy";

. \@ "dd/MMM/yyyy".

Note: Note: you can swap the d, M, y expressions around, but you must use uppercase 'M's for months - lowercase 'm's are for minutes.

• position the cursor anywhere in this field and press F9 to update it;

• run your mailmerge.
