## Coding conventions

We do not follow any published SQL coding standards, but we have established a set of basic coding standards to meet code consistency across our SQL repository.

**Please:**
* Use consistent and descriptive identifiers and names
* Make judicious use of white space and indentation to make code easier to read
* Indent code where necessary after keywords such as SELECT, FROM etc.
* Include comments in SQL where necessary - Use the C style opening `/* and */` to open multi-line comments and double hyphen `--` for single line comments

**Examples of good SQL coding standards:**

| Command            | Example                                                                                                                                                 |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|
| CREATE TABLE       | CREATE TABLE [transactions].[SALES](
                         CUST_ID INT NOT NULL,
                         SALE_ID INT NOT NULL,
                         QUANTITY INT NOT NULL,
                         PRIMARY KEY (CUST_ID, SALE_ID)
                       ) |
| SELECT             | SELECT
                        CUST_ID,
                        SALE_ID,
                        QUANTITY
                       FROM
                        [transactions].[SALES]
                       WHERE
                        SALE_ID = 1
                        AND QUANTITY > 2                      |
| CREATING VARIABLES | DECLARE
                        @CUSTOMER_REFERENCE INT = 1,
                        @EMAIL_TO VARCHAR(50) = 'DATA_MANAGEMENT@GLOBALSTORE.CO.UK'                                          |


Start reading our code to get a feel for it but most importantly, remember that this is open source software - consider the people who will read your code, and make it look nice for them.

🥂 Thank you! Team codon