---
title: Интеграция подключения к данным Microsoft Graph с управлением привилегированным доступом
description: Подключение к данным Microsoft Graph использует управление привилегированным доступом, чтобы позволить администраторам Microsoft 365 утверждать запросы на перемещение данных.
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 610b1abfb1d5e81cb7fc9a35bde98bed247fc143
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289318"
---
# <a name="microsoft-graph-data-connect-integration-with-privileged-access-management"></a>Интеграция подключения к данным Microsoft Graph с управлением привилегированным доступом

Подключение к данным Microsoft Graph использует управление привилегированным доступом (PAM), чтобы позволить администраторам Microsoft 365 утверждать запросы на перемещение данных. Конвейеры подключения к данным должны утверждаться участником группы утверждающих запросы на доступ к данным, который указывается администратором Microsoft 365 во время включения. Чтобы настроить группу утверждающих, см. статью [Начало работы](data-connect-get-started.md).

Каждому участнику группы утверждающих высылаются электронные письма с запросом на утверждение, чтобы уведомить их, когда действия копирования запрашивают доступ для извлечения данных Microsoft 365. Утверждающие могут утверждать или отклонять эти запросы, указывать группу пользователей, из которой следует удалить извлекаемые данные, или отозвать ранее утвержденный запрос. Утверждения сохраняются 6 месяцев, и требуется одно утверждение на каждое действие копирования в конвейере фабрики данных Azure. 

Каждый запрос всегда включает следующие сведения о наборе данных и пользователях, к которым относятся извлекаемые данные:

* **Запрашивающий**. Пользователь, запросивший конвейер.
* **Длительность**. Длительность сохранения утверждения (в случае утверждения). Всегда 4320 часов (6 месяцев).
* **Причина**. Причина запроса, обычно следующая: "Приложению, установленному для организации, требуется утверждение на доступ к данным Office 365".
* **Время запроса**. Дата и время запроса.
* **ИД запроса**. Идентификатор запроса для целей утверждения.
* **DataTable**. Набор извлекаемых данных (например, отправленные элементы).
* **Столбцы**. Список столбцов, извлекаемых из таблицы данных (например, SentDateTime).
* **AllowedGroups**. Группа или группы пользователей, данные которых извлекает конвейер. Если список групп пуст, конвейер запрашивает доступ к данным всех пользователей в клиенте.
* **Запрос области пользователей**. Предикат, используемый для фильтрации пользователей. Применяется только при запросе всех пользователей в клиенте. Если этот параметр пуст, фильтр не применяется. 
* **OutputUri**. Выходной путь, в котором хранятся извлеченные данные.
* **SourceTenantId**. Идентификатор клиента, из которого извлекаются данные.
* **InstallerIdentity**. Удостоверение установщика приложения.

Следующие поля в запросе доступны только в некоторых случаях:

* Имя приложения и URI Marketplace (доступно только для приложений, установленных из Azure Marketplace).
* Ссылки на политику конфиденциальности приложения и условия использования (доступны только при предоставлении приложением).
* Политики соответствия требованиям, применяемые приложением, например шифрование неактивных данных в выходном хранилище (доступны только при предоставлении приложением, и если приложение установлено из Azure Marketplace).
* Список запрещенных — группа пользователей, для которой может выполняться очистка извлеченных данных. Это поле не заполняется при запросе наборов данных, поддерживающих очистку извлеченных данных с целью обеспечения конфиденциальности. Оно может заполняться участником группы утверждающих, который утверждает запрос в соответствующее время. 

## <a name="approving-requests"></a>Утверждение запросов

Конвейеры подключения к данным должны утверждаться участником группы утверждающих запросы на доступ к данным. Утверждающие могут утверждать, отклонять или отзывать конвейеры с помощью модуля PowerShell для Exchange Online или пользовательского интерфейса PAM.

### <a name="approving-denying-and-revoking-requests-by-using-powershell"></a>Утверждение, отклонение и отзыв запросов с помощью PowerShell

Используйте следующие действия для взаимодействия с запросом с помощью модуля PowerShell для Exchange Online:

1. Установите модуль PowerShell для Exchange Online. Инструкции по установке см. в статье [Подключение к Exchange Online PowerShell с помощью многофакторной проверки подлинности](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).

2. Подключитесь к Exchange Online PowerShell с помощью многофакторной проверки подлинности (MFA). Инструкции см. в статье [Подключение к Exchange Online PowerShell с помощью многофакторной проверки подлинности](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).
    >**Примечание**. Вам не нужно включать многофакторную проверку подлинности для своей организации, чтобы использовать эти действия при подключении к Exchange Online PowerShell. Подключение с помощью многофакторной проверки подлинности создает маркер OAuth, используемый PAM для подписи ваших запросов.

3. Выполните вход с помощью своей учетной записи. Обратите внимание, что вы должны быть участником настроенной группы утверждающих доступ к данным, чтобы иметь возможность утверждать, отклонять или отзывать запросы. Гостевые пользователи не могут утверждать запросы, даже если они состоят в группе утверждающих. 

   ```powershell
   Connect-EXOPSSession
   ```

4. Найдите все ожидающие запросы.
   >**Примечание.** Значение свойства **Identity** будет использоваться для определения и утверждения или отклонения запроса. Запишите это значение и используйте его в параметре -RequestId. 

   ```powershell
   Get-ElevatedAccessRequest | ?{$_.RequestStatus -eq 'Pending'}
   ```

4. Подробнее ознакомьтесь с полем **context** нужного запроса. 
   >**Примечание.** Поле context запроса на доступ к данным описывает параметры и свойства действия копирования.

   ```powershell
   (Get-ElevatedAccessRequest -RequestId $requestId).Context | ConvertFrom-Json
   ```

   Вы получите примерно следующий ответ.

   ```powershell
   Key                          Value
   ---                          -----
   ApplicationName
   ComplianceStatus             [{"Timestamp":"2018-05-02T18:29:21.5705664Z","RequirementName":"adlsEncryption","PolicyComplianceState":"Compliant","Violations":0},{"Timestamp":"2018-05-02T...
   ApplicationMarketPlaceUri
   OutputUri                    adl://myadlserumvrroyspmq.azuredatalakestore.net/targetFolder/Event
   ApplicationPrivacyPolicyUri  http://www.wkw.com/privacy
   ApplicationTermsOfServiceUri http://www.wkw.com/tos
   InstallerIdentity            a89885c3-4b0e-499e-86ed-14d7ed9147c2@942229f8-4656-4fb0-828b-e938dad4019a
   SourceTenantId               942229f8-4656-4fb0-828b-e938dad4019a
   UserScopeQuery               tenant in (942229f8-4656-4fb0-828b-e938dad4019a)
   ApplicationId
   DataTable                    Calendar Events
   DestinationTenantId          942229f8-4656-4fb0-828b-e938dad4019a
   Columns                      Subject:string, HasAttachments:bool, End:DateTime, Start:DateTime, ResponseStatus:string, Organizer:Object, Attendees:string, Importance:string, Sensitivity:...
   ```

5. Утвердите или отклоните запрос, используя значение свойства **Identity** для параметра -RequestId.

   ```powershell
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!"
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

Также можно утвердить запрос с использованием списка запрещенных, чтобы не добавлять данные от определенных пользователей. Для этого нужно изменить контекст запроса, чтобы добавить параметр `object Id` группы, которую нужно пропустить, а затем утвердить запрос. 

   ```powershell
   $request = Get-ElevatedAccessRequest -RequestId
   $hash = $request.Context
   $hash["DenyList"] = <Object ID of denied user group>;
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!" -RequestContext $hash
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```
Кроме того, вы можете отозвать запросы, которые ранее были утверждены. Аналогично утверждению запросов потребуется значение свойства **Identity** для параметра -RequestId. 

   ```powershell 
   Revoke-ElevatedAccessAuthorization -Comment "Revoking this request!" -RequestId $requestId
   ```
   Ответ будет выглядеть приблизительно так:
   
   ```powershell
   AuthorizedBy          : user@tenant.onmicrosoft.com
   Type                  : Task
   AuthorizedAccess      : Data Access Request
   StartTimeUtc          : 7/24/2018 6:02:42 PM
   EndTimeUtc            : 10/22/2018 6:02:42 PM
   Revoked               : True
   RevocationDateTimeUtc : 7/24/2018 9:12:55 PM
   RevokedBy             : NAMPR00A001.prod.outlook.com/Microsoft Exchange Hosted  Organizations/tenant.onmicrosoft.com/user
   RevocationComment     : Revoking this request!
   Identity              : bda75607-0d87-43cb-bdf1-284b18446b34
   DateCreatedUtc        : 1/1/0001 12:00:00 AM
   DateUpdatedUtc        : 7/24/2018 9:12:55 PM
   ```

### <a name="approving-denying-and-revoking-requests-by-using-the-pam-user-experience"></a>Утверждение, отклонение и отзыв запросов с помощью пользовательского интерфейса PAM

Используйте следующие действия для взаимодействия с запросом с помощью веб-интерфейса PAM:

1. Войдите на портал администрирования Microsoft 365, используя учетные данные администратора, и перейдите на страницу [пользовательского интерфейса утверждения управления привилегированным доступом](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess). Будут показаны все запросы на доступ (ожидаемые, утвержденные, истекшие или отклоненные).

На открывшейся странице выберите нужный запрос. Чтобы выбрать список запрещенных с целью очистки для обеспечения конфиденциальности, щелкните раскрывающийся **список запрещенных**, выберите группу, которую нужно очистить, и нажмите **Утвердить**.

Чтобы отозвать ранее утвержденный запрос, выберите его и нажмите **Отозвать**. Следующая попытка перенести данные с помощью этого утверждения завершится сбоем. 

### <a name="approval-behavior"></a>Поведение при утверждении

Запросы на утверждение подключения к данным имеют определенные характеристики, которые важно учитывать:

- Запросы на утверждение основаны на именах фабрики данных Azure, конвейера и действия копирования. При каждом запуске копирования выполняется проверка того, что администратор Microsoft 365 утвердил запрос действия копирования на доступ к данным Office, а также проверка важных параметров действия копирования относительно параметров утверждения.
- При определенных условиях автоматически выполняется новый запрос на утверждение. Утверждающий подключение к данным должен утвердить новый запрос перед тем, как действие копирования сможет получить доступ к данным Microsoft 365.
- Если параметры выполняемого копирования изменяются, выполняется новый запрос на утверждение.
- Если изменяются имена фабрики данных, конвейера или действия копирования, выполняется новый запрос на утверждение.
- Например: потребуется новое утверждение, если изменяется таблица данных или набор столбцов, к которым обращается действие копирования.
- Действия копирования требуется утверждать каждые 6 месяцев. Если исходное утверждение получено 6 месяцев назад, автоматически выполняется новый запрос на утверждение.
- Если утверждающий запросы на доступ к данным Microsoft 365 отклонил запрос на утверждение или отозвал ранее утвержденный запрос, действие копирования будет постоянно завершаться сбоем. Вам следует в сотрудничестве с утверждающим выяснить причину отклонения или отзыва и соответствующим образом исправить параметры действия копирования. Потребуется развернуть новое действие копирования или изменить имя существующего действия копирования, чтобы выполнить новый запрос на утверждение.
- Запрос на утверждение истекает через 24 часа, если утверждающий запросы на доступ к данным Microsoft 365 не выполняет действий с запросом. Новый запрос отправляется на утверждение каждые 24 часа. Если вы видите, что ваше действие копирования ожидает утверждения (на этапе ожидания согласия), в сотрудничестве с утверждающими запросы на доступ к данным Microsoft 365 получите утверждение для вашего запроса.

## <a name="privacy-scrubbing"></a>Очистка для обеспечения конфиденциальности 
Участник группы утверждающих, который утверждает запрос, может указать имя одной группы пользователей, данные которых будут очищены от извлеченных данных. Строки, содержащие адреса электронной почты, соответствующие участникам запрещенной группы, будут очищены от извлеченных данных. Группы, вложенные в запрещенную группу, будут развернуты, и очистка будет выполняться только для пользователей. Сведения о применении списка запрещенных во время утверждения с помощью PowerShell или пользовательского интерфейса PAM см. в разделе об утверждении запросов в этой статье. 

В следующей таблице представлены имена наборов данных и столбцов, для которых выполняется проверка содержимого с целью очистки для обеспечения конфиденциальности.

| Имя набора данных                     | Столбцы, используемые для очистки на основе списка запрещенных                                                  |
|---------------------------------------------------------------------|----------------------------------------------------------|
| **BasicDataSet_v0.Message_v0**<br>**BasicDataSet_v0.Message_v1**   | Sender, From, ToRecipients, CcRecipients, BccRecipients    |                                                                               
| **BasicDataSet_v0.SentItem_v0**<br>**BasicDataSet_v0.SentItem_v1**  | Sender, From, ToRecipients, CcRecipients, BccRecipients  |
| **BasicDataSet_v0.Event_v0**<br>**BasicDataSet_v0.Event_v1**     | Organizer, Attendees                                        |
| **BasicDataSet_v0.Contact_v0**<br>**BasicDataSet_v0.Contact_v1**  | EmailAddresses                                            |
| **BasicDataSet_v0.CalendarView_v0**                                | Organizer, Attendees                                      |

## <a name="next-steps"></a>Дальнейшие действия

Убедитесь, что в вашей организации правильно настроено управление привилегированным доступом для использования с данными Microsoft Graph, выполнив действия, указанные в статье [Начало работы](data-connect-get-started.md).