# MySQL Advanced

This repository contains advanced MySQL projects focusing on stored procedures, triggers, views, and indexing techniques. These projects are designed to enhance database optimization skills and performance tuning.

## Project Overview

This project covers:
- Creating and using unique indexes
- Creating and using stored procedures
- Creating and using views
- Creating and using triggers
- Working with advanced table constraints
- Performance optimization with indexes

## Tasks

### 0. We are all unique!
- Creates a table with unique email constraint
- Enforces business rules directly in the schema
- File: `0-uniq_users.sql`

### 1. In and not out
- Creates a table with enumeration constraints for country field
- Demonstrates the use of ENUM data type
- File: `1-country_users.sql`

### 2. Best band ever!
- Ranks country origins of bands by number of fans
- Demonstrates data aggregation techniques
- File: `2-fans.sql`

### 3. Old school band
- Lists bands with Glam rock as their main style
- Shows computation with date-based fields
- File: `3-glam_rock.sql`

### 4. Buy buy buy
- Creates a trigger to decrease item quantity after adding an order
- Shows automation of related table updates
- File: `4-store.sql`

### 5. Email validation to sent
- Creates a trigger to reset email validation only when email changes
- Demonstrates conditional trigger execution
- File: `5-valid_email.sql`

### 6. Add bonus
- Creates a stored procedure to add new corrections for students
- Shows parameter handling and conditional logic
- File: `6-bonus.sql`

### 7. Average score
- Creates a stored procedure to compute and store average scores
- Shows computation and storage of derived data
- File: `7-average_score.sql`

### 8. Optimize simple search
- Creates an index on the first letter of names
- Demonstrates performance optimization for text searches
- File: `8-index_my_names.sql`

### 9. Optimize search and score
- Creates a composite index on name first letter and score
- Shows multi-column indexing strategy
- File: `9-index_name_score.sql`

### 10. Safe divide
- Creates a function to safely handle division operations
- Shows error handling in SQL functions
- File: `10-div.sql`

### 11. No table for a meeting
- Creates a view for students needing meetings
- Shows view creation with complex conditions
- File: `11-need_meeting.sql`

### 12. Average weighted score (Advanced)
- Creates a stored procedure to compute weighted average scores
- Shows more complex computation with joins
- File: `100-average_weighted_score.sql`

### 13. Average weighted score for all! (Advanced)
- Creates a stored procedure to compute weighted scores for all students
- Shows batch processing in stored procedures
- File: `101-average_weighted_score.sql`

## Environment
- All files executed on Ubuntu 18.04 LTS using MySQL 5.7
- SQL keywords written in uppercase
- Each SQL query preceded by a comment describing the task

## Usage
Files can be executed as follows:
```
$ cat [filename] | mysql -uroot -p [database]
```

## Author
Shighi
