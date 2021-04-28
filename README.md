# SQL

WORLD Challenges

1. SELECT COUNT(*) FROM city WHERE CountryCode = "USA";
- 274

2. SELECT population,lifeexpectancy FROM country WHERE name="Argentina";
- Population - 37032000
- Life Expectancy - 75.1

3. SELECT * FROM country WHERE LifeExpectancy IS NOT NULL ORDER BY LifeExpectancy DESC LIMIT 5;
- Andorra, 83.5

4. SELECT c.Name, cn.Name, c.Capital FROM country c JOIN city cn ON c.Capital = cn.ID WHERE c.name = "Spain";
- Spain, Madrid, id 653

5. SELECT DISTINCT cl.Language FROM country c LEFT OUTER JOIN countrylanguage cl ON c.code = cl.countrycode WHERE region = "Southeast Asia";
- 47 results

6. SELECT* FROM city WHERE name LIKE "f%" LIMIT 25;

7. SELECT COUNT(*) FROM country c JOIN city cn ON c.code = cn.CountryCode WHERE c.name = "China";
- 363 results

8. SELECT * FROM country WHERE Population IS NOT NULL AND Population > "1" ORDER BY Population ASC LIMIT 5;
- Pitcairn, 50 people

9. SELECT COUNT(DISTINCT Code) FROM country;
- 239

10. SELECT * FROM country ORDER BY SurfaceArea DESC Limit 10;

11. SELECT Name, Population, CountryCode FROMcity WHERE CountryCode = "JPN" ORDER BY population DESC LIMIT 5;
- Tokyo, Yokohama, Osaka, Nagoya, Sapporo

12. UPDATE country SET HeadOfState = "Elizabeth II" WHERE HeadOfState = "Elisabeth II"
SELECT * FROM country WHERE headofstate LIKE "Eli%";
- 35 countries found

13. SELECT Name, Population/SurfaceArea FROM country WHERE Population/SurfaceArea > "1" ORDER BY Population/SurfaceArea DESC LIMIT 10;
- Macao, Monaco, HK, SG, Gibraltar, Holy See, Bermuda, Malta, Maldives, Bangladesh

14. SELECT DISTINCT language FROM countrylanguage;
- 457 results

15. SELECT Name, GNP FROM country ORDER BY GNP DESC LIMIT 10;
- US, JPN, GER, FR, UK, ITA, CHN, BR, Canada, Spain

16.= ????????????????

17. SELECT CountryCode FROM countrylanguage WHERE language = "German" AND Percentage >50; (Incomplete, need to join country code with other table).
