---
ms.localizationpriority: medium
ms.openlocfilehash: 3c4731d0d1b8f6f7015387fee6a59e3a3d8f1883
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768235"
---
<!-- markdownlint-disable MD002 MD041 -->

Администратор Microsoft 365 может утверждать или отклонять запросы на согласие. Это можно сделать через центр Microsoft 365 Admin или программным способом с помощью PowerShell.

## <a name="approve-consent-requests"></a>Утверждение запросов на согласие

# <a name="microsoft-365-admin-center"></a>[Microsoft 365 Admin Center](#tab/Microsoft365)

1. Откройте браузер и перейдите на портал [Microsoft 365 Admin.](https://admin.microsoft.com)

1. Чтобы утвердить или отклонить запросы на согласие, перейдите к [privileged Access](https://portal.office.com/adminportal/home#/Settings/PrivilegedAccess).

1. Выберите ожидающий **запрос на доступ к данным**.

1. В **вызове запроса на** доступ к данным нажмите кнопку **"Утвердить** ".

    ![Снимок экрана: запрос на доступ к данным, ожидающий утверждения согласия в Центр администрирования Microsoft 365.](../concepts/images/data-connect-m365-approve.png)

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

1. Откройте Windows PowerShell.
1. Убедитесь, что сеанс PowerShell включил сценарии с удаленной подписью.

    ```powershell
    Set-ExecutionPolicy RemoteSigned
    ```

1. Подключитесь к Exchange Online.

    1. Получите учетные данные для входа, выполнив следующую команду PowerShell. Войдите с помощью пользователя, отличного от того, который создал и запустил конвейер Фабрика данных Azure, с примененной ролью **глобальный администратор**, членом группы, которая имеет права на утверждение запросов к данным в Microsoft 365 и имеет включенную многофакторную проверку подлинности.

        ```powershell
        $UserCredential = Get-Credential
        ```

    1. Создайте новый Exchange Online PowerShell и загрузите (импортируйте) его.

        ```powershell
        $Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://ps.protection.outlook.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection
        Import-PSSession $Session -DisableNameChecking
        ```

        > [!IMPORTANT]
        > Завершив этот сеанс, убедитесь, что вы отключались от сеанса с помощью команды PowerShell `Remove-PSSession $Session`. Exchange Online три открытых удаленных сеанса PowerShell для защиты от атак типа "отказ в обслуживании" (DoS). Если просто закрыть окно PowerShell, подключение не будет открыто.

1. Получите список всех ожидающих запросов данных из подключения к данным Microsoft Graph, выполнив следующую команду PowerShell.

    ```powershell
    Get-ElevatedAccessRequest | where {$_.RequestStatus -eq 'Pending'} | select RequestorUPN, Service, Identity, RequestedAccess | fl
    ```

    - Изучите список возвращенных запросов на доступ к данным. На следующем рисунке обратите внимание, что есть два ожидающих запроса.

        ![Снимок экрана: список ожидающих запросов, отформатированных в виде списка в консоли PowerShell.](../concepts/images/data-connect-ps-pending-requests.png)

1. Утвердите доступ к данным, возвращенный на предыдущем шаге, скопируйте идентификатор GUID запроса, выполнив следующую команду PowerShell.

    > [!NOTE]
    > Замените GUID в следующем фрагменте кода идентификатором GUID из результатов предыдущего шага.

    ```powershell
    Approve-ElevatedAccessRequest -RequestId fa041379-0000-0000-0000-7cd5691484bd -Comment 'approval request granted'
    ```

1. Через несколько секунд вы увидите страницу состояния обновления выполнения действия, чтобы показать, что теперь _выполняется извлечение данных_.

    ![Снимок экрана: портал Azure пользовательского интерфейса для службы фабрики данных, где состояние загрузки теперь отображается как "Извлечение данных".](../concepts/images/data-connect-adf-extraction-approved.png)

1. Этот процесс извлечения данных может занять некоторое время в зависимости от размера клиента Microsoft 365.

---

## <a name="verify-extracted-data-from-microsoft-365-to-azure-storage-blob"></a>Проверка извлеченных данных из Microsoft 365 в большой двоичный объект службы хранилища Azure

1. Откройте браузер и перейдите на портал [Azure](https://portal.azure.com/).

1. Войдите с помощью учетной **записи с глобальный администратор** правами на доступ к клиентам Azure и Microsoft 365.

1. На боковой панели навигации выберите пункт меню **"Все** ресурсы".

1. В списке ресурсов выберите учетную запись хранения **Azure** , созданную ранее в этом руководстве.

1. В меню навигации на боковой панели выберите большие двоичные **объекты** в колонке учетной **записи хранения Azure** .

1. Выберите контейнер **,** созданный ранее в этом руководстве, Фабрика данных Azure конвейера в качестве приемника для извлеченных данных. Вы должны увидеть данные в этом контейнере.

    ![Снимок экрана: портал Azure пользовательского интерфейса для службы учетной записи хранения. Здесь показан контейнер, в котором хранятся извлеченные данные.](../concepts/images/data-connect-adf-extracted-data-in-blob.png)
