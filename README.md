1. Expectation Suite Name ods_billing

Table-Level Expectations
Must have exactly 6 columns.	Проверка кол-ва колонок
Must have these columns in this order: user_id, billing_period, service, tariff, sum, created_at	Проверка что все колонки в наличие

billing_period
values must never be null.	Проверка что значения не null
values must match this regular expression: [0-9]{4}-[0-9]{2}.	Проверка соответствия маске
created_at
values must never be null.	Проверка что значения не null
service
values must never be null.	Проверка что значения не null
sum
values must never be null.	Проверка что значения не null
values must be greater than or equal to 0.01.	Проверка на значение
tariff
values must never be null.	Проверка что значения не null
distinct values must belong to this set: Mini Maxi Gigabyte Megabyte.	Проверка что значения из списка
distinct values must match this set: Mini Maxi Gigabyte Megabyte.	Проверка что все значения из списка есть (поскольку сет большой)
user_id
values must never be null.	Проверка что значения не null
must have greater than or equal to 2 unique values.	Проверка что сет не содержит только 1 значение

2. Expectation Suite Name ods_issue
 
Table-Level Expectations
Must have exactly 6 columns.	Проверка кол-ва колонок
Must have these columns in this order: user_id, start_time, end_time, title, description, service	Проверка что все колонки в наличие
 
description
values must never be null.	Проверка что значения не null
end_time
values must never be null.	Проверка что значения не null
service
distinct values must belong to this set: Setup Environment Connect Disconnect.	Проверка что значения из списка
distinct values must match this set: Setup Environment Connect Disconnect.	Проверка что все значения из списка есть (поскольку сет большой)
start_time
values must never be null.	Проверка что значения не null
title
values must never be null.	Проверка что значения не null
user_id
values must never be null.	Проверка что значения не null
must have greater than or equal to 2 unique values.	Проверка что сет не содержит только 1 значение

3. Expectation Suite Name ods_traffic

Table-Level Expectations
Must have exactly 6 columns.	Проверка кол-ва колонок
Must have these columns in this order: user_id, timestamp, device_id, device_ip_addr, bytes_sent, bytes_received	Проверка что все колонки в наличие

bytes_received
values must never be null.	Проверка что значения не null
values must be greater than or equal to 0.	проверка на значение
bytes_sent
values must never be null.	Проверка что значения не null
values must be greater than or equal to 0.	проверка на значение
device_id
values must never be null.	Проверка что значения не null
values must match this regular expression: d[0-9]{3}.	Проверка соответствия шаблону
device_ip_addr
values must never be null.	Проверка что значения не null
values must match this regular expression: [0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.[0-9]{1,3}.	Проверка соответствия шаблону
timestamp
values must never be null.	Проверка что значения не null
user_id
values must never be null.	Проверка что значения не null
must have greater than or equal to 2 unique values.	Проверка что сет не содержит только 1 значение

4. Expectation Suite Name araev.ods_payment.warning

Table-Level Expectations
Must have exactly 8 columns.	Проверка кол-ва колонок
Must have these columns in this order: user_id, pay_doc_type, pay_doc_num, account, phone, billing_period, pay_date, sum	Проверка что все колонки в наличие


account
values must never be null.	Проверка что значения не null
values must match this regular expression: FL-[0-9]..	Проверка соответствия шаблону
billing_period
values must never be null.	Проверка что значения не null
values must match this regular expression: [0-9]{4}-[0-9]{2}.	Проверка соответствия шаблону
pay_date
values must never be null.	Проверка что значения не null
pay_doc_num
values must never be null.	Проверка что значения не null
values must be greater than or equal to 1.
pay_doc_type
values must never be null.	Проверка что значения не null
distinct values must belong to this set: MASTER MIR VISA.	Проверка что значения из списка
distinct values must match this set: MASTER MIR VISA.	Проверка что все значения из списка есть (поскольку сет большой)
sum
values must never be null.	Проверка что значения не null
values must be greater than or equal to 1.	Проверка на значение
user_id
values must never be null.	Проверка что значения не null
must have greater than or equal to 2 unique values.	Проверка что сет не содержит только 1 значение

