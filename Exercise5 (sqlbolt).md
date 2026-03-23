# SQL LAB (sqlbolt)- Exercise 5
## 1. List all the Canadian cities and their populations
```sql
SELECT city, population 
FROM north_american_cities 
WHERE country = 'Canada';
```
# Output
| city        | population |
|-------------|------------|
| Toronto     | 2615060    |
| Montreal    | 1649519    |
| Vancouver   | 603502     |

## 2. Order all the cities in the United States by their latitude from north to south
```sql
SELECT city, latitude 
FROM north_american_cities 
WHERE country = 'United States' 
ORDER BY latitude DESC;
```
# Output
| city        | latitude |
|-------------|----------|
| Chicago     | 41.8781  |
| New York    | 40.7128  |
| Los Angeles | 34.0522  |
| Houston     | 29.7604  |
| Phoenix     | 33.4484  |

## 3. List all the cities west of Chicago, ordered from west to east
```sql
SELECT city, longitude 
FROM north_american_cities 
WHERE longitude < -87.6298 
ORDER BY longitude ASC;
```
# Output
| city        | longitude |
|-------------|-----------|
| Vancouver   | -123.1207 |
| Los Angeles | -118.2437 |
| Phoenix     | -112.0740 |
| Houston     | -95.3698  |

## 4. List the two largest cities in Mexico (by population)
```sql
SELECT city, population 
FROM north_american_cities 
WHERE country = 'Mexico' 
ORDER BY population DESC 
LIMIT 2;
```
# Output
| city        | population |
|-------------|------------|
| Mexico City | 8555500    |
| Guadalajara | 1495182    |

## 5. List the third and fourth largest cities (by population) in the United States and their population
```sql
SELECT city, population 
FROM north_american_cities 
WHERE country = 'United States' 
ORDER BY population DESC 
LIMIT 2 OFFSET 2;
```
# Output
| city    | population |
|---------|------------|
| Chicago | 2718782    |
| Houston | 2195914    |
