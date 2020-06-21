---
title: Известные проблемы с Microsoft Graph
description: В этой статье описываются известные проблемы, связанные с Microsoft Graph.
author: MSGraphDocsVTeam
localization_priority: Priority
ms.openlocfilehash: 98c61991ec99b1f7776c03f5fa5bc2400b5950a6
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744053"
---
# <a name="known-issues-with-microsoft-graph"></a>Известные проблемы с Microsoft Graph

В этой статье описываются известные проблемы, связанные с Microsoft Graph. 

Чтобы сообщить о известной проблеме, посетите страницу [поддержки Microsoft Graph](https://developer.microsoft.com/graph/support) .

Сведения о последних обновлениях API Microsoft Graph можно найти в [журнале изменений Microsoft Graph](changelog.md).

## <a name="bookings"></a>Bookings

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a>Ошибка ErrorExceededFindCountLimit при запросе bookingBusinesses

При получении списка по запросу `bookingBusinesses` возвращается ошибка с указанным ниже кодом, если у организации есть несколько компаний в Bookings, а учетная запись, с использованием которой отправлен запрос, не принадлежит администратору.

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

В качестве обходного решения можно ограничить группу компаний, возвращаемых по запросу, указав параметр `query`. Пример:

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendars"></a>Календари

### <a name="accessing-a-shared-calendar"></a>Доступ к общему календарю

При использовании следующей операции для доступа к событиям в календаре другого пользователя:

```http
GET /users/{id}/calendars/{id}/events
```

You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:

- Существуют два способа реализации общего доступа к календарю, которые для ясности мы будем называть "старый" способ и "новый" способ.
- Новый способ в настоящее время доступен для предоставления доступа к календарям с разрешениями на просмотр или редактирование, но не с делегированными разрешениями.
- С помощью REST API календаря можно просматривать и редактировать общие календари, только если доступ к ним предоставлен **новым** способом.
- С помощью REST API календаря нельзя просматривать или редактировать общие календари (или их события), если доступ к ним предоставлен **старым** способом.


Если доступ к календарю был предоставлен с разрешениями на просмотр или редактирование, но старым способом, вы можете вручную обновить календарь, чтобы использовать новый способ.
Чтобы можно было использовать новый способ, со временем Outlook автоматически обновит все общие календари, в том числе те, доступ к которым предоставлен с делегированными разрешениями.

Чтобы с этой целью вручную обновить общий календарь, выполните следующие действия:
1.  Получатель удаляет календарь, доступ к которому был ранее ему предоставлен.
2.  Владелец повторно предоставляет доступ к календарю в Outlook в Интернете, Outlook на iOS или Outlook на Android.
3.  The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)
4.  Доступ к календарю успешно предоставлен новым способом, если получатель может просмотреть его в Outlook на iOS или Outlook на Android.

A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:

```http
GET /me/calendars/{id}/events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>Добавление календарей ICS в почтовый ящик пользователя и доступ к ним

В настоящее время календари ICS поддерживаются частично:

* Вы можете добавить календарь ICS в почтовый ящик пользователя через интерфейс пользователя, но не через API Microsoft Graph.
* [Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.
* Вы также можете [отобразить события](/graph/api/calendar-list-events?view=graph-rest-1.0) календаря ICS.

### <a name="attaching-large-files-to-events"></a>Прикрепление больших файлов к событиям
Приложение с делегированными разрешениями возвращает `HTTP 403 Forbidden` при попытке [присоединить большие файлы](outlook-large-attachments.md) к сообщению Outlook или событию, которое находится в общем или делегированном почтовом ящике. С делегированными разрешениями [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) завершается успешно, только если сообщение или событие находятся в почтовом ящике вошедшего в систему пользователя.

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a>Поддержка свойства onlineMeetingUrl для Microsoft Teams

В настоящее время свойство **onlineMeetingUrl** ресурса [event](/graph/api/resources/event?view=graph-rest-1.0) для собрания Skype означает URL-адрес для собрания по сети. Однако для ресурса event собрания в Microsoft Teams задано значение NULL.

В бета-версии предлагается обходное решение, позволяющее использовать свойство **onlineMeetingProvider** ресурса [event](/graph/api/resources/event?view=graph-rest-beta) с целью убедиться, что поставщиком является Microsoft Teams. С помощью свойства **onlineMeeting** ресурса **event** вы можете получить доступ к объекту **joinUrl**.

## <a name="change-notifications"></a>Уведомления об изменениях

### <a name="additional-notifications-for-users"></a>Дополнительные уведомления для пользователей

[Подписки](/graph/api/resources/subscription) на изменения для **пользователя** с **changeType**, для которого установлено значение **обновлено**, также будут получать уведомления о **changeType**: **обновлено** при создании пользователя и обратимом удалении пользователя.

### <a name="additional-notifications-for-groups"></a>Дополнительные уведомления для групп

[Подписки](/graph/api/resources/subscription) на изменения для **группы** с **changeType**, для которого установлено значение **обновлено**, также будут получать уведомления о **changeType**: **обновлено** при создании группы и обратимом удалении группы.

## <a name="cloud-communications"></a>Облачные коммуникации 

Клиент Microsoft Teams не отображает меню **Просмотреть сведения о собрании** для собраний канала, созданных с помощью API коммуникаций из облака.

## <a name="cloud-solution-provider-apps"></a>Приложения Cloud Solution Provider

### <a name="csp-apps-must-use-azure-ad-endpoint"></a>Приложения CSP должны использовать конечную точку Azure AD

Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a>В некоторых клиентах предоставленные приложениям CSP разрешения не работают

Предоставленные приложениям CSP разрешения могут не работать в некоторых клиентах.

- После первого входа в приложение, использующее делегированные разрешения, в новом клиенте может возникнуть эта ошибка: `AADSTS50000: There was an error issuing a token`.
- Приложение, использующее разрешения для приложений, может получить маркер, но ему может быть неожиданно отказано в доступе при вызове Microsoft Graph.

Мы делаем все возможное, чтобы как можно быстрее исправить эту ошибку.

Для целей разработки и тестирования можно использовать следующее временное решение.

>**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.

1. Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. Создайте субъект-службу Microsoft Graph.

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="contacts"></a>Контакты

### <a name="organization-contacts-available-in-only-beta"></a>Контакты организации доступны только в бета-версии

Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.

### <a name="default-contacts-folder"></a>Папка контактов по умолчанию

В версии `/v1.0` запрос `GET /me/contactFolders` не включает папку контактов пользователя по умолчанию.

A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

В указанном выше запросе:

1. `/me/contacts?$top=1` возвращает свойства [контакта](/graph/api/resources/contact?view=graph-rest-1.0) в папке контактов по умолчанию.
2. При добавлении `&$select=parentFolderId` возвращается только свойство контакта **parentFolderId** — идентификатор папки контактов по умолчанию.


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a>Доступ к контактам через папку контактов в бета-версии

В настоящее время в версии `/beta` существует проблема, из-за которой нельзя получить доступ к ресурсу [contact](/graph/api/resources/contact?view=graph-rest-beta), указав его родительскую папку в URL-адресе запроса REST, как показано в 2 приведенных ниже сценариях.

* Доступ к контакту из папки верхнего уровня [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta).

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

Кроме того, вы можете просто [получить](/graph/api/contact-get?view=graph-rest-beta) контакт по его идентификатору, как показано ниже, так как конечная точка /contacts для запроса GET в версии `/beta` применяется ко всем контактам в почтовом ящике пользователя:

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a>Разностный запрос

* При отслеживании изменений в отношениях иногда неправильно возвращается контекст OData.
* Расширения схемы (устаревшие) не возвращаются с оператором $select и возвращаются без него.
* Клиенты не могут отслеживать изменения в открытых расширениях и зарегистрированных расширениях схемы.

## <a name="extensions"></a>Расширения

### <a name="change-tracking-is-not-supported"></a>Отслеживание изменений не поддерживается

Отслеживание изменений не поддерживается для свойств открытых расширений и расширений схемы.

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a>Одновременное создание ресурса и открытого расширения

You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a>Создание экземпляра ресурса с одновременным добавлением данных расширения схемы

Вы не можете указать расширение схемы в той же операции, которая создает экземпляр **contact**, **event**, **message** или **post**.
Сперва нужно создать экземпляр ресурса, а затем выполнить операцию `PATCH` для этого экземпляра, чтобы добавить расширение схемы и пользовательские данные.

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a>Для каждого экземпляра ресурса разрешено не более 100 значений свойства расширения схемы

В настоящее время для каждого экземпляра таких ресурсов каталога, как **device**, **group** и **user**, можно установить не более 100 значений свойства расширения схемы.

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a>Фильтрация по свойствам расширения схемы поддерживается не для всех типов объектов

Фильтрация по свойствам расширения схемы (с помощью выражения `$filter`) не поддерживается для типов объектов Outlook **contact**, **event**, **message** или **post**.

## <a name="files-onedrive"></a>Файлы (OneDrive)

* При первом доступе к личному диску пользователя с помощью Microsoft Graph до открытия им своего личного сайта в браузере возвращается ответ 401.

## <a name="groups"></a>Группы

### <a name="permissions-for-groups-and-microsoft-teams"></a>Разрешения для групп и Microsoft Teams

Microsoft Graph предоставляет два разрешения ([*Group.Read.All*](permissions-reference.md#group-permissions) и [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) для доступа к API для групп и Microsoft Teams.
Эти разрешения должен предоставить администратор.
В будущем мы планируем добавить новые разрешения для групп и команд, которые смогут предоставлять пользователи.

Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.

Примеры функций групп, поддерживающих разрешения только для приложений и делегированные разрешения:

* создание и удаление групп;
* получение и обновление свойств групп, связанных с администрированием групп и управлением ими;
* синхронизация, типы и [параметры каталогов](/graph/api/resources/directoryobject?view=graph-rest-1.0) групп;
* владельцы и члены групп.
* Извлечение групповых бесед и потоков

Примеры функций групп, поддерживающих только делегированные разрешения:

* События групп, Фото
* внешние отправители, разрешенные или запрещенные отправители, подписка на группы;
* избранное пользователей и счетчик непросмотренных элементов.

### <a name="policy"></a>Политика

С помощью Microsoft Graph можно создать группу Office 365 и присвоить ей название в обход всех групповых политик Office 365, настроенных через Outlook Web App.

### <a name="setting-the-allowexternalsenders-property"></a>Установка свойства allowExternalSenders

В настоящее время существует проблема, из-за которой невозможно установить свойство **allowExternalSenders** группы в операции POST или PATCH как в `/v1.0`, так и в `/beta`.

### <a name="using-delta-query"></a>Работа с запросами изменений

Об известных проблемах, связанных с запросом изменений, можно узнать в [соответствующем разделе](#delta-query) этой статьи.

## <a name="identity-and-access--application-and-service-principal-apis"></a>Удостоверение и доступ | API приложений и субъектов-служб

There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development. The following is a summary of current limitations and in-development API features.

Текущие ограничения:

* Некоторые свойства application (такие как appRoles и addIns) будут доступны только после внесения всех изменений.
* Регистрировать можно только мультитенантные приложения.
* Обновлять можно только приложения, зарегистрированные после первоначального обновления бета-версии.
* Пользователи Azure Active Directory могут регистрировать приложения и добавлять владельцев.
* Поддержка протоколов OpenID Connect и OAuth.
* Невозможно назначение политик приложению.
* Не выполняются операции с ownedObjects, для которых требуется код appId (например, users/{id|userPrincipalName}/ownedObjects/{id}/...).

В разработке:

* Возможность регистрировать однотенантные приложения.
* Обновления объекта servicePrincipal.
* Перевод существующих приложений Azure AD на обновленную модель.
* Поддержка appRoles, предварительно авторизованные клиенты, необязательные утверждения, утверждения членства в группе и брендинг.
* Пользователи учетной записи Майкрософт (MSA) могут регистрировать приложения.
* Поддержка протоколов SAML и WsFed.

## <a name="identity-and-access--conditional-access"></a>Удостоверение и доступ | Условный доступ

### <a name="permissions"></a>Разрешения

В настоящее время для вызова API POST и PATCH требуется разрешение Policy.Read.All. В дальнейшем разрешение Policy.ReadWrite.ConditionalAccess позволит читать политики из каталога.

## <a name="json-batching"></a>Пакетная обработка JSON

### <a name="no-nested-batch"></a>Не поддерживаются вложенные пакеты

Пакетные запросы JSON не должны содержать вложенных пакетных запросов.

### <a name="all-individual-requests-must-be-synchronous"></a>Все отдельные запросы должны быть синхронными

All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.

### <a name="no-transactions"></a>Не поддерживается диалоговая обработка

Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.

### <a name="uris-must-be-relative"></a>URI должны быть относительными

Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.

### <a name="limit-on-batch-size"></a>Ограничение на размер пакета

В настоящее время в пакетный запрос JSON можно включить не более 20 отдельных запросов.

### <a name="simplified-dependencies"></a>Упрощенные зависимости

Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:

1. Параллельный — для отдельных запросов не указаны зависимости в свойстве `dependsOn`.
2. Последовательный — все отдельные запросы зависят от предыдущего отдельного запроса.
3. Идентичный — для всех отдельных запросов в свойстве `dependsOn` указана одна и та же зависимость.

После усовершенствования пакетной обработки JSON эти ограничения будут удалены.

## <a name="mail-outlook"></a>Почта (Outlook)

### <a name="attaching-large-files-to-messages"></a>Вложение больших файлов в сообщения
Приложение с делегированными разрешениями возвращает `HTTP 403 Forbidden` при попытке [присоединить большие файлы](outlook-large-attachments.md) к сообщению Outlook или событию, которое находится в общем или делегированном почтовом ящике. С делегированными разрешениями [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) завершается успешно, только если сообщение или событие находятся в почтовом ящике вошедшего в систему пользователя.

### <a name="the-comment-parameter-for-creating-a-draft"></a>Параметр comment для создания черновика

Параметр **comment** для создания ответа или черновика ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) не включается в текст полученного черновика сообщения.

### <a name="get-messages-returns-chats-in-microsoft-teams"></a>При использовании запроса GET для сообщений возвращаются также чаты в Microsoft Teams

В конечных точках версии 1 и бета-версии данные отклика для `GET /users/id/messages` включают чаты Microsoft Teams, не входящие в область группы или канала. Тема этих сообщений чата: "IM".

## <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

### <a name="get-teams-is-not-supported"></a>GET / команды не поддерживается

Чтобы получить список команд, см. [список всех команд](teams-list-all-teams.md) и [список ваших команд](/graph/api/user-list-joinedteams?view=graph-rest-1.0).

### <a name="post-teams-is-only-available-in-beta"></a>POST / команды доступны только в бета-версии
Чтобы создавать команды в версии 1.0, ознакомьтесь со статьей [Создание группы](/graph/api/team-put-teams?view=graph-rest-1.0).

### <a name="missing-teams-in-list-all-teams"></a>Отсутствующие команды в списке всех команд

Некоторые команды, созданные в прошлом, но не использовавшиеся в последнее время пользователем Microsoft Teams, не указываются при использовании метода [перечисления всех команд](teams-list-all-teams.md).
Новые команды будут перечислены.
У некоторых старых команд нет свойства **resourceProvisioningOptions**, содержащего значение "Team", которое присваивается недавно созданным командам и командам, посещаемым в Microsoft Teams.
В будущем свойство **resourceProvisioningOptions** будет присваиваться существующим командам, не открывавшимся в Microsoft Teams.

## <a name="users"></a>Пользователи

### <a name="no-instant-access-after-creation"></a>Нет мгновенного доступа после создания

Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.

### <a name="photo-restrictions"></a>Ограничения для фотографий

Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource.
Failure to read or update a photo, in this case, would result in the following error:

```javascript
{
  "error": {
    "code": "ErrorNonExistentMailbox",
    "message": "The SMTP address has no mailbox associated with it."
  }
}
```

### <a name="using-delta-query"></a>Запрос изменений

Об известных проблемах, связанных с запросом изменений, можно узнать в [соответствующем разделе](#delta-query) этой статьи.

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a>Отзыв сеансов входа возвращает неправильный код HTTP

[user: revokeSignInSessions API](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) должен возвращать ответ `204 No content` в случае успешного отзыва и код ошибки HTTP (4xx или 5xx), если запрос не выполнен.    Однако из-за проблемы со службой этот API возвращает `200 OK` и логический параметр, который всегда правильный.  Пока проблема не будет устранена, разработчикам рекомендуется просто интерпретировать код возврата 2xx как успешное выполнение запроса к этому API.

### <a name="incomplete-objects-when-using-getbyids-request"></a>Неполные объекты при использовании запроса getByIds

При запросе объектов с помощью [получения объектов каталога из списка идентификаторов](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) должны возвращаться полные объекты. Однако в настоящее время объекты [user](/graph/api/resources/user?view=graph-rest-1.0) в конечной точке версии 1.0 возвращаются с ограниченным набором свойств. Временное решение: возврат более полных объектов [user](/graph/api/resources/user?view=graph-rest-1.0) обеспечивается при использовании операции в сочетании с параметром запроса `$select`. Это поведение не соответствует спецификациям OData. Так как это поведение может быть изменено в будущем, используйте это временное решение только при указании в параметре `$select=` всех нужных свойств и только если допускается внесение существенных изменений в это временное решение.

## <a name="query-parameter-limitations"></a>Ограничения параметров запроса

* Не поддерживается несколько пространств имен.
* Не поддерживаются запросы GET для `$ref` и приведение для пользователей, групп, устройств, субъектов-служб и приложений.
* `@odata.bind` is not supported.  This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.
* Отсутствует `@odata.id` для навигации по объектам без вложений (например, сообщениям) при использовании минимальных метаданных.
* `$expand`:
  * Отсутствует поддержка `nextLink`.
  * Поддерживается не более одного уровня развертывания.
  * Не поддерживаются дополнительные параметры (`$filter`, `$select`).
* `$filter`:
  * Конечная точка `/attachments` не поддерживает фильтры. При ее наличии параметр `$filter` игнорируется.
  * Фильтрация нескольких рабочих нагрузок не поддерживается.
* `$search`:
  * Полнотекстовый поиск доступен только для некоторых объектов, например сообщений.
  * Поиск по нескольким рабочим нагрузкам не поддерживается.


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a>Функции, доступные только в REST API Office 365 или API Graph Azure AD

Некоторые функции еще не доступны в Microsoft Graph. Если вы не нашли нужную функцию, можете использовать специальные [REST API Office 365](https://docs.microsoft.com/previous-versions/office/office-365-api/). Сведения об Azure Active Directory см. в статье [Миграция приложений Azure AD Graph в Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview). 
