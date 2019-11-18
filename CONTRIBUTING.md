## Coding conventions

We do not follow any published SQL coding standards, but we have established a set of basic coding standards to meet code consistency across our SQL repository.

**Please:**
* Use consistent and descriptive identifiers and names
* Make judicious use of white space and indentation to make code easier to read
* Indent code where necessary after keywords such as SELECT, FROM etc.
* Include comments in SQL where necessary - Use the C style opening `/* and */` to open multi-line comments and double hyphen `--` for single line comments

**Examples of good SQL coding standards:**

Creating a table:

    CREATE TABLE [transactions].[SALES](
        CUST_ID INT NOT NULL,
        SALE_ID INT NOT NULL,
        QUANTITY INT NOT NULL,
        PRIMARY KEY (CUST_ID, SALE_ID)
    )

Select statement:

    SELECT
        CUST_ID,
        SALE_ID,
        QUANTITY
    FROM
        [transactions].[SALES]
    WHERE
        SALE_ID = 1
        AND QUANTITY > 2

Creating variables:

    DECLARE
        @CUSTOMER_REFERENCE INT = 1,
        @EMAIL_TO VARCHAR(50) = 'DATA_MANAGEMENT@GLOBALSTORE.CO.UK'


Start reading our code to get a feel for it but most importantly, remember that this is open source software - consider the people who will read your code, and make it look nice for them.

## Code of Conduct

As a contributer you can help us keep the Codon community open and inclusive. Please read and follow our [Code of Conduct](https://github.com/codonlibrary/code-of-conduct/tree/master). By contributing to it, you agree to comply with it.

🥂 Thank you! Team codon