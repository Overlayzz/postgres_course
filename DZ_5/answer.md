**1. PgBouncer pool_mode = session**

Не перевожу PgBouncer в режим session, т.к. он по дефолту.

Работа PgBouncer в режиме session:

![img.png](img.png)

**2. PgBouncer pool_mode = transaction**

Перевожу PgBouncer в режим transaction:

![img_1.png](img_1.png)

Работа PgBouncer в режиме transaction:

![img_2.png](img_2.png)

**3. PgBouncer pool_mode = statement**

Перевожу PgBouncer в режим statement:

![img_3.png](img_3.png)

Работа PgBouncer в режиме statement:

![img_4.png](img_4.png)

Результаты тестирования производительности показали следующее:
1) Наиболее эффективный режим — statement.
2) Средний уровень производительности — transaction, немного уступает режиму statement.
3) Наименее производительный режим — session.