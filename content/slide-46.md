# Part 2: Querying and Modifying Complex Data

## DML

UPDATE replaces a document that already exists with updated values

The example on the right changes the type of the document "baldwin" from 
"contact" to "actor"

<pre id="example">
UPDATE contacts 
    SET type = "actor" 
      WHERE META(contacts).id = "baldwin"
      RETURNING contacts
</pre>
