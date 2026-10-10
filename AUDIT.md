# перевірка

## Перевірка за критеріями
 Критерій                    Результат      Примітка 
 AC-1 PK `<сутність>_id`, int    ок  
 AC-2 FK = PK за назвою й типом  ок       `publisher_id`, `book_id`, `reader_id`, `copy_id` 
 AC-3 3NF                        ок        похідних атрибутів немає 
 AC-4 чисті M:N без junction     ок        R2, R3 — прямі зв'язки 
 AC-5 асоціативна лише LOAN      ок        LOAN має власні атрибути 
 AC-6 назви spec ↔ model         ок        `scripts/check_consistency.py` 
 AC-7 кардинальності             ок        збігаються з R1–R6 
 AC-8 UK позначені               ок        `isbn`, `inventory_number`, `email` 
