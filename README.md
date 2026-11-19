# Финансовый менеджер

CLI утилита на джаве для управления и расчета финансов.

## Архитектура
```console 
financialManagement/
└──app/
    ├── pom.xml
    ├── data/
    │   ├── users.csv
    │   ├── categories.csv
    │   ├── transactions.csv
    │   └── budgets.csv
    │
    ├── src/
    │   ├── main/
    │   │   ├── java/com/finance/
    │   │   │   ├── cli/
    │   │   │   │   ├── Main.java
    │   │   │   │   ├── CommandProcessor.java
    │   │   │   │   ├── ConsoleFormatter.java
    │   │   │   │   └── command/
    │   │   │   │       ├── Command.java
    │   │   │   │       ├── HelpCommand.java
    │   │   │   │       ├── RegisterCommand.java
    │   │   │   │       ├── LoginCommand.java
    │   │   │   │       ├── LogoutCommand.java
    │   │   │   │       ├── CategoryAddCommand.java
    │   │   │   │       ├── CategoryListCommand.java
    │   │   │   │       ├── CategoryRenameCommand.java
    │   │   │   │       ├── CategoryDeleteCommand.java
    │   │   │   │       ├── IncomeCommand.java
    │   │   │   │       ├── ExpenseCommand.java
    │   │   │   │       ├── TransactionDeleteCommand.java
    │   │   │   │       ├── BudgetSetCommand.java
    │   │   │   │       ├── BudgetEditCommand.java
    │   │   │   │       ├── BudgetShowCommand.java
    │   │   │   │       ├── StatsCommand.java
    │   │   │   │       ├── TransferCommand.java
    │   │   │   │       ├── ExportCommand.java
    │   │   │   │       ├── ImportCommand.java
    │   │   │   │       ├── SaveCommand.java
    │   │   │   │       └── ExitCommand.java
    │   │   │   │
    │   │   │   ├── model/
    │   │   │   │   ├── User.java
    │   │   │   │   ├── Wallet.java
    │   │   │   │   ├── Category.java
    │   │   │   │   ├── Transaction.java
    │   │   │   │   ├── Budget.java
    │   │   │   │   └── TransactionType.java
    │   │   │   │
    │   │   │   ├── dao/
    │   │   │   │   ├── UserDao.java
    │   │   │   │   ├── WalletDao.java
    │   │   │   │   ├── CategoryDao.java
    │   │   │   │   ├── TransactionDao.java
    │   │   │   │   ├── BudgetDao.java
    │   │   │   │   └── csv/
    │   │   │   │       ├── CsvUtils.java
    │   │   │   │       ├── CsvUserDao.java
    │   │   │   │       ├── CsvCategoryDao.java
    │   │   │   │       ├── CsvTransactionDao.java
    │   │   │   │       ├── CsvBudgetDao.java
    │   │   │   │       └── CsvWalletDao.java
    │   │   │   │
    │   │   │   ├── service/
    │   │   │   │   ├── AuthService.java
    │   │   │   │   ├── CategoryService.java
    │   │   │   │   ├── TransactionService.java
    │   │   │   │   ├── BudgetService.java
    │   │   │   │   ├── StatisticsService.java
    │   │   │   │   ├── AlertService.java
    │   │   │   │   ├── TransferService.java
    │   │   │   │   └── ReportService.java
    │   │   │   │
    │   │   │   └── util/
    │   │   │       ├── InputValidator.java
    │   │   │       ├── MoneyUtils.java
    │   │   │       └── PasswordHasher.java
    │   │   └── resources/
    │   │       └── TODO
    │   │
    │   └── test/
    │       └── java/com/finance/
    │           └── TODO
```