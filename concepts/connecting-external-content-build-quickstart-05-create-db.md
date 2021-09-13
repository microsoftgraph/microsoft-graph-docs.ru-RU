---
ms.localizationpriority: medium
ms.openlocfilehash: e8f13a3fe886db688d12a997f0cddc38547a30f6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289668"
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
