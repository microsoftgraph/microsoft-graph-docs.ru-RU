---
ms.localizationpriority: medium
ms.openlocfilehash: e8f13a3fe886db688d12a997f0cddc38547a30f6
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805410"
---
<!-- markdownlint-disable MD002 MD025 MD041 -->

1. Откройте интерфейс командной строки (CLI) в каталоге, где расположен PartsInventoryConnector.csproj.
2. Выполните следующие команды:

  ```dotnetcli
  dotnet ef migrations add InitialCreate
  dotnet ef database update
  ```

> [!NOTE]
> Запустите следующие команды, если схема изменяется в CSV-файле и отражают эти изменения в базе данных SQLite.

```dotnetcli
dotnet ef database drop
dotnet ef database update
```
