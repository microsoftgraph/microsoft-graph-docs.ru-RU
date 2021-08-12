<!-- markdownlint-disable MD002 MD041 -->

Администратор Microsoft 365 может утверждать или отказывать в запросах на согласие. Это можно сделать через центр Microsoft 365 Admin или программным путем с помощью PowerShell.

## <a name="approve-consent-requests"></a>Утверждение запросов на согласие

# <a name="microsoft-365-admin-center"></a>[Microsoft 365 Admin Центр](#tab/Microsoft365)

1. Откройте браузер и перейдите на [портал Microsoft 365 Admin.](https://admin.microsoft.com)

1. Чтобы утверждать или отказывать в запросах на согласие, перейдите в [привилегированный доступ](https://portal.office.com/adminportal/home#/Settings/PrivilegedAccess).

1. Выберите ожидающих **запрос на доступ к данным.**

1. В **вызове запроса на доступ к данным** выберите кнопку **Утверждение.**

    ![Снимок экрана, на котором показан запрос на доступ к данным до утверждения согласия в Центр администрирования Microsoft 365.](images/data-connect-m365-approve.png)

# <a name="powershell"></a>[PowerShell](#tab/PowerShell)

1. Откройте Windows PowerShell.
1. Убедитесь, что сеанс PowerShell включил удаленно подписанные скрипты.

    ```powershell
    Set-ExecutionPolicy RemoteSigned
    ```

1. Подключение Exchange Online.

    1. Получение входа в учетные данные, исполнив следующую PowerShell. Во включай использование другого пользователя, создавшего и затеявшего конвейер Azure Data Factory, который имеет роль глобального администратора, который входит в группу, которая имеет права утверждать запросы на данные в Microsoft 365 и имеет многофакторную проверку подлинности. 

        ```powershell
        $UserCredential = Get-Credential
        ```

    1. Создайте новый сеанс Exchange Online PowerShell и загрузим его (импорт).

        ```powershell
        $Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://ps.protection.outlook.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection
        Import-PSSession $Session -DisableNameChecking
        ```

        > [!IMPORTANT]
        > После завершения этого сеанса убедитесь, что вы отключались от сеанса с помощью команды `Remove-PSSession $Session` PowerShell. Exchange Online позволяет использовать только три открытых сеанса удаленной powerShell для защиты от атак с отказом в обслуживании (DoS). Если просто закрыть окно PowerShell, оно оставит подключение открытым.

1. Получите список всех ожидающих запросов данных из Подключение к данным Microsoft Graph, исполнив следующую PowerShell.

    ```powershell
    Get-ElevatedAccessRequest | where {$_.RequestStatus -eq 'Pending'} | select RequestorUPN, Service, Identity, RequestedAccess | fl
    ```

    - Изучите список возвращенных запросов на доступ к данным. На следующем изображении обратите внимание на два ожидающих запроса.

        ![Снимок экрана, на котором показан список ожидающих запросов, отформатированный в виде списка на консоли PowerShell.](images/data-connect-ps-pending-requests.png)

1. Утверждение доступа к данным, возвращенного на предыдущем шаге, скопируйте GUID удостоверения запроса, исполнив следующую PowerShell.

    > [!NOTE]
    > Замените GUID в следующем фрагменте кода на GUID по результатам предыдущего шага.

    ```powershell
    Approve-ElevatedAccessRequest -RequestId fa041379-0000-0000-0000-7cd5691484bd -Comment 'approval request granted'
    ```

1. Через несколько минут вы увидите страницу состояния для обновления запуска действий, чтобы показать, что она теперь _извлекает данные._

    ![Снимок экрана, на котором показан пользовательский интерфейс портала Azure для службы Фабрика данных, где состояние нагрузки теперь отображается как "Извлечение данных".](images/data-connect-adf-extraction-approved.png)

1. Этот процесс извлечения данных может занять некоторое время в зависимости от размера Microsoft 365 клиента.

---

## <a name="verify-extracted-data-from-microsoft-365-to-azure-storage-blob"></a>Проверка извлеченных данных из Microsoft 365 до служба хранилища Azure Blob

1. Откройте браузер и перейдите на портал [Azure.](https://portal.azure.com/)

1. Впишитесь в использование учетной записи **с правами глобального** администратора для клиентов Azure и Microsoft 365.

1. На боковой панели навигации выберите элемент **меню "Все** ресурсы".

1. В списке ресурсов выберите учетную **запись служба хранилища Azure, созданную** ранее в этом руководстве.

1. В меню навигации на боковой панели выберите **Blobs** из служба хранилища Azure **учетной записи.**

1. Выберите **контейнер,** созданный ранее в этом руководстве, который вы настроили конвейер Azure Data Factory в качестве раковины для извлеченных данных. Вы должны видеть данные в этом контейнере сейчас.

    ![Снимок экрана, на котором показан пользовательский интерфейс портала Azure для служба хранилища учетной записи. Он показывает контейнер, в котором хранятся извлеченные данные.](images/data-connect-adf-extracted-data-in-blob.png)
