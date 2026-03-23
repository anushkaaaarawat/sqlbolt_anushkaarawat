# SQL LAB (sqlbolt)- EXercise 2
## 1.Find all the Toy Story movies
```sql
SELECT * 
FROM movies 
WHERE title LIKE 'Toy Story%';
```
# Output
| id | title        | director        | year | length_minutes |
|----|--------------|-----------------|------|----------------|
| 1  | Toy Story    | John Lasseter   | 1995 | 81             |
| 3  | Toy Story 2  | John Lasseter   | 1999 | 93             |
| 11 | Toy Story 3  | Lee Unkrich     | 2010 | 103            |

## 2. Find all the movies directed by John Lasseter
```sql
SELECT * 
FROM movies 
WHERE director = 'John Lasseter';
```
# Output
| id | title        | director        | year | length_minutes |
|----|--------------|-----------------|------|----------------|
| 1  | Toy Story    | John Lasseter   | 1995 | 81             |
| 2  | A Bug's Life | John Lasseter   | 1998 | 95             |
| 3  | Toy Story 2  | John Lasseter   | 1999 | 93             |
| 7  | Cars         | John Lasseter   | 2006 | 117            |
| 12 | Cars 2       | John Lasseter   | 2011 | 120            |

## 3. Find all the movies (and director) not directed by John Lasseter
```sql
SELECT title, director 
FROM movies 
WHERE director <> 'John Lasseter';
```
# Output
| title               | director        |
|---------------------|-----------------|
| Monsters, Inc.      | Pete Docter     |
| Finding Nemo        | Andrew Stanton  |
| The Incredibles     | Brad Bird       |
| Ratatouille         | Brad Bird       |
| WALL-E              | Andrew Stanton  |
| Up                  | Pete Docter     |
| Toy Story 3         | Lee Unkrich     |
| Brave               | Brenda Chapman  |
| Monsters University | Dan Scanlon     |

## 4. Find all the WALL-* movies
```sql
SELECT * 
FROM movies 
WHERE title LIKE 'WALL-%';
```
# Output
| id | title  | director        | year | length_minutes |
|----|--------|-----------------|------|----------------|
| 9  | WALL-E | Andrew Stanton  | 2008 | 104            |
