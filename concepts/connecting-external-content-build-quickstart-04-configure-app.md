---
ms.localizationpriority: medium
ms.openlocfilehash: e04c28e801be69487d83e5b5a3184c4702652aa3
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805365"
---
<!-- markdownlint-disable MD002 MD025 MD041 -->

1. Откройте интерфейс командной строки (CLI) в каталоге, где расположен PartsInventoryConnector.csproj.
2. Запустите следующую команду, чтобы инициализировать секреты пользователя для проекта.

    ```dotnetcli
    dotnet user-secrets init
    ```

3. Запустите следующие команды для хранения вашего ID приложения, секрета приложения и ИД клиента в хранилище секрета пользователя.

    ```dotnetcli
      dotnet user-secrets set appId "YOUR_APP_ID_HERE"
      dotnet user-secrets set appSecret "YOUR_APP_SECRET_HERE"
      dotnet user-secrets set tenantId "YOUR_TENANT_ID_HERE"
    ```
