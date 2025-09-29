# Module-5-Assignment

Question 1
----------
Problem: The code uses a simple lookup to locate data regardless of user's access permissions.
Solution: Enforcing role-based access control will prevent a malicious actor from accessing privileged information.

Question 2
----------
Problem: The code does not require a password in order to log into the system. Therefore, anyone with knowledge of a user_id can access that user's account.
Solution: Implement password protections. (For simplification, the password variable in the solution code is not encrypted and is submitted as raw text; in the real world, the password would need to be processed through an encryption algorithm.)

Question 3
----------
Problem: The code uses the MD5 algorithm, which has been deprecated due to poor security and a higher chance for a hash collision compared with SHA256.
Solution: Use SHA256 in place of MD5.

Question 4
----------
Problem: The code uses the SHA1 algorithm, which has been deprecated due to a small hash size of 160 bytes as well as a greater chance of a hash collision compared to other hash algorithms.
Solution: Use SHA256 in place of SHA1.

Question 5
----------
Problem: The username variable is appended to the end of the query, which allows for code to be injected into the query.
Solution: Enforce input validation by using a prepared statement.

Question 6
----------
Problem: The code does not use parameterized queries and thus could be subject to SQL injection.
Solution: Use parameterized queries to prevent SQL injection.

Question 7
----------
Problem: The code does not encrypt password data, and as a result it is not stored in an encrypted state within the database.
Solution: Providing encryption of all passwords should be part of the standard implementation.

Question 8
----------
Problem: The full library is able to be accessed.
Solution: Loading only the necessary files will prevent malicious actors from accessing the full software library.

Question 9
----------
Problem: The URL supplied by the user is not validated and thus could be used by an attacker to force a request to a different destination.
Solution: Sanitize the user input by enforicng a whitelist of URLs that can be accessed. *Ideally, the user interface would supply whitelisted URLs by means of a combobox or some other form of whitelist presentation.

Question 10
----------
Problem: The user is not identified nor authenticated, thus the code is vulnerable to credential stuffing and brute-force attacks.
Solution: Enforce authentication of the user by issuing a unique, randomly-generated user ID to each user.
