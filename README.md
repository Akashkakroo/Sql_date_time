# Sql_date_time

1/ orders
CREATE TABLE orders (
  order_id INT PRIMARY KEY,
  customer_id INT,
  order_date DATE,
  order_time TIME,
  delivered_at TIMESTAMP
);


INSERT INTO orders VALUES
(1, 101, '2025-05-20', '09:15:00', '2025-05-20 11:45:00'),
(2, 102, '2025-05-21', '13:45:00', '2025-05-21 16:30:00'),
(3, 103, '2025-05-22', '07:10:00', '2025-05-22 14:00:00'),
(4, 104, '2025-05-23', '10:30:00', '2025-05-23 13:00:00'),
(5, 105, '2025-05-24', '08:00:00', NULL);



2/ user_activity
CREATE TABLE user_activity (
  user_id INT,
  activity_date DATE,
  login_time TIMESTAMP
);


INSERT INTO user_activity VALUES
(101, '2025-05-20', '2025-05-20 08:30:00'),
(102, '2025-05-21', '2025-05-21 11:00:00'),
(103, '2025-05-22', '2025-05-22 07:00:00'),
(101, '2025-05-23', '2025-05-23 09:45:00'),
(104, '2025-05-24', '2025-05-24 12:00:00');
