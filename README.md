# OrangeHRM Manual QA (Learning Project)

**Manual Testing Practice | Test Design Techniques | Work in Progress**

Учебный проект по ручному тестированию HR-платформы **OrangeHRM** (демо-версия). Цель проекта — попробовать протестировать незнакомую ранее функциональность и применить на практике различные техники тест-дизайна: эквивалентное разбиение, граничные значения, попарное тестирование и другие. Проект не завершён и не претендует на полное покрытие приложения — часть модулей протестирована подробно, часть осталась за скобками.

---

# Application Under Test

**Website:** https://opensource-demo.orangehrmlive.com

На данный момент были протестированы следующие модули:

* Authentication (Login, Forgot Password)
* Dashboard
* Admin — User Management
* PIM — Add Employee, Data Import, Optional Fields
* Leave — Leave List
* Buzz — Newsfeed

Полный список модулей приложения (включая непротестированные) описан в `application-overview.md`.

---

# Project Structure

```
├── application-overview.md          # Обзор функциональности приложения
├── bug-reports/                     # Баг-репорты
│   └── auth-13.md
├── checklists/                      # Чек-листы по модулям
│   ├── authentication-checklist.md
│   └── dashboard-checklist.md
└── test-suites/                     # Тест-кейсы по модулям
    ├── admin/
    │   └── user-management.md
    ├── buzz/
    │   └── newsfeed.md
    ├── leave/
    │   └── leave-list.md
    └── pim/
        ├── add-employee.md
        ├── data-import.md
        └── optional-fields.md
```

---

# What I Practiced

* **Анализ приложения** — разбор функциональности незнакомого продукта перед тестированием ([`application-overview.md`](application-overview.md)).
* **Чек-листы** — быстрая проверка модулей Authentication и Dashboard ([`checklists/`](checklists)).
* **Детализированные тест-кейсы** — Test Data, Preconditions, Steps, Expected Result, Postconditions по модулям Admin, PIM, Leave и Buzz ([`test-suites/`](test-suites)).
* **Техники тест-дизайна** — эквивалентное разбиение, граничные значения, комбинирование условий при составлении тест-кейсов (например, фильтрация в Admin → User Management, длина текста поста в Buzz).
