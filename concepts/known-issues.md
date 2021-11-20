---
title: Известные проблемы с Microsoft Graph
description: В этой статье описываются известные проблемы, связанные с Microsoft Graph.
author: MSGraphDocsVTeam
ms.localizationpriority: high
ms.openlocfilehash: e0e6ac6237d9d6dce6d5ec786b69d6faaba8b814
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123581"
---
# <a name="known-issues-with-microsoft-graph"></a>Известные проблемы с Microsoft Graph

В этой статье описываются известные проблемы, связанные с Microsoft Graph. 

Чтобы сообщить об известных проблемах, перейдите на[поддержки Microsoft Graph](https://developer.microsoft.com/graph/support).

Сведения о последних обновлениях API в Microsoft Graph см. в [журнале изменений Microsoft Graph](changelog.md).

## <a name="applications"></a>Приложения

### <a name="some-limitations-apply-to-the-application-and-serviceprincipal-resources"></a>Некоторые ограничения применяются к ресурсам приложения и servicePrincipal

Изменения в ресурсах [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) и [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) в настоящее время находятся в разработке. Ниже приведено краткое описание текущих ограничений и возможностей API, находящихся в разработке.

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

### <a name="azure-ad-v20-endpoint-is-not-supported-for-csp-apps"></a>Конечная точка Azure AD v2.0 не поддерживается для приложений CSP

Приложения CSP должны получать маркеры из конечных точек Azure AD (версии 1) для успешного вызова Microsoft Graph в своих клиентах, управляемых партнерами. В настоящее время получение маркера через конечную точку Azure AD версии 2.0 не поддерживается.

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a>В некоторых клиентах предоставленные приложениям CSP разрешения не работают

При определенных обстоятельствах предварительное согласие для приложений поставщика облачных решений (CSP) может не работать для некоторых ваших клиентов.

- После первого входа в приложение, использующее делегированные разрешения, в новом клиенте может возникнуть эта ошибка: `AADSTS50000: There was an error issuing a token`.
- Приложение, использующее разрешения для приложений, может получить маркер, но ему может быть неожиданно отказано в доступе при вызове Microsoft Graph.

Мы делаем все возможное, чтобы как можно быстрее исправить эту ошибку.

Для целей разработки и тестирования можно использовать следующее временное решение.

>**ПРИМЕЧАНИЕ.** Это не окончательное решение и предназначено только для целей разработки. Оно станет ненужным после исправления упомянутой выше ошибки. Удалять указанный ниже субъект-службу не нужно.

1. Откройте сеанс Azure AD PowerShell 2 и подключитесь к клиенту `customer`, введя учетные данные администратора в окне входа. Скачать и установить Azure AD PowerShell 2 можно [здесь](https://www.powershellgallery.com/packages/AzureAD).

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. Создайте субъект-службу Microsoft Graph.

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="bookings"></a>Bookings

### <a name="error-when-querying-bookingbusinesses"></a>Ошибка при запросе bookingBusinesses

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

```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendar"></a>Календарь

### <a name="error-accessing-a-shared-calendar"></a>Ошибка при доступе к общему календарю

При использовании следующей операции для доступа к событиям в календаре другого пользователя:

```http
GET /users/{id}/calendars/{id}/events
```

Может возникнуть ошибка HTTP 500 `ErrorInternalServerTransientError`. Ошибка возникает, потому что:

- Существуют два способа реализации общего доступа к календарю, которые для ясности мы будем называть "старый" способ и "новый" способ.
- Новый способ в настоящее время доступен для предоставления доступа к календарям с разрешениями на просмотр или редактирование, но не с делегированными разрешениями.
- С помощью REST API календаря можно просматривать и редактировать общие календари, только если доступ к ним предоставлен **новым** способом.
- С помощью REST API календаря нельзя просматривать или редактировать общие календари (или их события), если доступ к ним предоставлен **старым** способом.


Если доступ к календарю был предоставлен с разрешениями на просмотр или редактирование, но старым способом, вы можете вручную обновить календарь, чтобы использовать новый способ.
Чтобы можно было использовать новый способ, со временем Outlook автоматически обновит все общие календари, в том числе те, доступ к которым предоставлен с делегированными разрешениями.

Чтобы с этой целью вручную обновить общий календарь, выполните следующие действия:
1.  Получатель удаляет календарь, доступ к которому был ранее ему предоставлен.
2.  Владелец повторно предоставляет доступ к календарю в Outlook в Интернете, Outlook на iOS или Outlook на Android.
3.  Получатель повторно принимает календарь, используя Outlook в Интернете. (Скоро можно будет использовать другие клиенты Outlook.)
4.  Доступ к календарю успешно предоставлен новым способом, если получатель может просмотреть его в Outlook на iOS или Outlook на Android.

Календарь, доступ к которому предоставлен новым способом, выглядит как один из стандартных календарей в вашем почтовом ящике. С помощью REST API календаря можно просматривать и редактировать события в общем календаре, как в своем собственном. Например:

```http
GET /me/calendars/{id}/events
```

### <a name="partial-support-for-adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>Частичная поддержка добавления календарей ICS в почтовый ящик пользователя и доступа к ним

В настоящее время календари на основе подписки на интернет-календарь (ICS) поддерживаются только частично:

* Вы можете добавить календарь ICS в почтовый ящик пользователя через интерфейс пользователя, но не через API Microsoft Graph.
* [Перечисление календарей пользователя](/graph/api/user-list-calendars) позволяет получить свойства **name**, **color** и **id** всех [календарей](/graph/api/resources/calendar) в группе календарей пользователя по умолчанию или указанной группе календарей, в том числе календарей ICS. URL-адрес ICS невозможно хранить и открывать в ресурсе calendar.
* Вы также можете [отобразить события](/graph/api/calendar-list-events) календаря ICS.

### <a name="error-attaching-large-files-to-events"></a>Ошибка при прикреплении больших файлов к событиям
Приложение с делегированными разрешениями возвращает `HTTP 403 Forbidden` при попытке [присоединить большие файлы](outlook-large-attachments.md) к сообщению Outlook или событию, которое находится в общем или делегированном почтовом ящике. С делегированными разрешениями [createUploadSession](/graph/api/attachment-createuploadsession) завершается успешно, только если сообщение или событие находятся в почтовом ящике вошедшего в систему пользователя.

### <a name="onlinemeetingurl-property-is-not-supported-for-microsoft-teams"></a>Свойство onlineMeetingUrl не поддерживается для Microsoft Teams

В настоящее время свойство **onlineMeetingUrl** ресурса [event](/graph/api/resources/event) для собрания Skype означает URL-адрес для собрания по сети. Однако для ресурса event собрания в Microsoft Teams задано значение NULL.

В бета-версии предлагается обходное решение, позволяющее использовать свойство **onlineMeetingProvider** ресурса [event](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) с целью убедиться, что поставщиком является Microsoft Teams. С помощью свойства **onlineMeeting** ресурса **event** вы можете получить доступ к объекту **joinUrl**.

## <a name="change-notifications"></a>Уведомления об изменениях

### <a name="update-notifications-occur-on-creation-and-soft-deletion-of-users"></a>Уведомления об обновлении возникают при создании и обратимом удалении пользователей

[Подписки](/graph/api/resources/subscription) на изменения для **пользователя** с **changeType**, для которого установлено значение **обновлено**, также будут получать уведомления о **changeType**: **обновлено** при создании пользователя и обратимом удалении пользователя.

### <a name="update-notifications-occur-on-creation-and-soft-deletion-of-groups"></a>Уведомления об обновлении возникают при создании и обратимом удалении групп

[Подписки](/graph/api/resources/subscription) на изменения для **группы** с **changeType**, для которого установлено значение **обновлено**, также будут получать уведомления о **changeType**: **обновлено** при создании группы и обратимом удалении группы.

## <a name="cloud-communications"></a>Облачные коммуникации 

### <a name="view-meeting-details-menu-is-not-available-on-microsoft-teams-client"></a>Меню "Просмотр сведений о собрании" недоступно в клиенте Microsoft Teams

Клиент Microsoft Teams не отображает меню **Просмотреть сведения о собрании** для собраний канала, созданных с помощью API коммуникаций из облака.

## <a name="compliance"></a>Соответствие требованиям

### <a name="subject-rights-request-api-permissions-are-not-currently-available"></a>Разрешения API запроса прав субъекта в настоящее время недоступны

Объекты API запроса прав субъекта в API конфиденциальности Microsoft Graph в настоящее время не имеют доступных разрешений. Эта проблема может помешать пользователям видеть разрешения и давать согласие на использование API в своей среде. 

## <a name="contacts"></a>Контакты

### <a name="get-operation-does-not-return-default-contacts-folder"></a>Операция GET не возвращает папку контактов по умолчанию

В версии `/v1.0` запрос `GET /me/contactFolders` не включает папку контактов пользователя по умолчанию.

Эта ошибка будет исправлена. Чтобы получить идентификатор папки контактов по умолчанию, вы можете использовать следующий запрос на [отображение контактов](/graph/api/user-list-contacts) и свойство **parentFolderId**:

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

В этом запросе:

1. `/me/contacts?$top=1` возвращает свойства [контакта](/graph/api/resources/contact) в папке контактов по умолчанию.
2. При добавлении `&$select=parentFolderId` возвращается только свойство контакта **parentFolderId** — идентификатор папки контактов по умолчанию.


### <a name="accessing-contacts-via-a-contact-folder-doesnt-work-in-beta"></a>Доступ к контактам через папку контактов не работает в бета-версии

В настоящее время в версии `/beta` существует проблема, из-за которой нельзя получить доступ к ресурсу [contact](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true), указав его родительскую папку в URL-адресе запроса REST, как показано в 2 приведенных ниже сценариях.

Доступ к контакту из пользовательской [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta&preserve-view=true) верхнего уровня:

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

Доступ к контакту в дочерней папке папки **contactFolder**: 

```http
GET /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

В предыдущем примере показан один уровень вложения, но для хранения контакта допускается несколько.

Кроме того, вы можете просто [получить](/graph/api/contact-get?view=graph-rest-beta&preserve-view=true) контакт по его идентификатору, как показано ниже, так как конечная точка /contacts для запроса GET в версии `/beta` применяется ко всем контактам в почтовом ящике пользователя:

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a>Разностный запрос

### <a name="odata-context-is-returned-incorrectly"></a>Контекст OData возвращается неправильно

При отслеживании изменений в отношениях иногда неправильно возвращается контекст OData.

### <a name="schema-extensions-are-not-returned-with-select"></a>Расширения схемы не возвращаются с `select`

Расширения схемы (устаревшие) не возвращаются с оператором `$select`, но возвращаются без `$select`.

### <a name="clients-cannot-track-changes-to-open-extensions"></a>Клиенты не могут отслеживать изменения в открытых расширениях

Клиенты не могут отслеживать изменения в открытых расширениях и зарегистрированных расширениях схемы.

## <a name="devices-and-apps--device-updates-windows-updates"></a>Устройства и приложения | Обновления устройств (обновления Windows)

### <a name="accessing-and-updating-deployment-audiences-is-not-supported"></a>Доступ к аудиториям развертывания и их обновление не поддерживаются

Доступ к аудиториям развертывания и их обновление для ресурсов **deployment**, созданных с помощь Intune, в настоящее время не поддерживается.

* [Перечисление членов аудитории развертывания](/graph/api/windowsupdates-deploymentaudience-list-members) и [перечисление исключений из аудитории развертывания](/graph/api/windowsupdates-deploymentaudience-list-exclusions) возвращает `404 Not Found`.
* [Обновление состава и исключений из аудитории развертывания](/graph/api/windowsupdates-deploymentaudience-updateaudience) или [обновление по идентификатору](/graph/api/windowsupdates-deploymentaudience-updateaudiencebyid) возвращает `202 Accepted`, но аудитория не обновляется.

## <a name="extensions"></a>Расширения

### <a name="change-tracking-is-not-supported"></a>Отслеживание изменений не поддерживается

Отслеживание изменений не поддерживается для свойств открытых расширений и расширений схемы.

### <a name="unable-to-create-a-resource-and-open-extension-at-the-same-time"></a>Не удалось создать ресурс и открытое расширение одновременно

Невозможно указать открытое расширение при создании экземпляра **administrativeUnit**, **device**, **group**, **organization** или **user**. Сначала необходимо создать экземпляр, а затем указать данные открытого расширения в последующем запросе ``POST`` к этому экземпляру.

### <a name="unable-to-create-a-resource-instance-and-add-schema-extension-data-at-the-same-time"></a>Не удалось создать экземпляр ресурса с одновременным добавлением данных расширения схемы

Вы не можете указать расширение схемы в той же операции, которая создает экземпляр **contact**, **event**, **message** или **post**.
Сперва нужно создать экземпляр ресурса, а затем выполнить операцию `PATCH` для этого экземпляра, чтобы добавить расширение схемы и пользовательские данные.

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a>Для каждого экземпляра ресурса разрешено не более 100 значений свойства расширения схемы

В настоящее время для каждого экземпляра таких ресурсов каталога, как **device**, **group** и **user**, можно установить не более 100 значений свойства расширения схемы.

### <a name="owner-must-be-specified-when-updating-a-schemaextension-definition-using-microsoft-graph-explorer"></a>При обновлении определения schemaExtension с помощью проводника Microsoft Graph должен быть указан владелец

При использовании `PATCH` для обновления schemaExtension с помощью проводника Graph необходимо указать свойство **owner** и задать для него текущее значение `appid` (которое должно быть `appId` имеющегося приложения). Это также относится к любому клиентскому приложению `appId`, **владелец** которого не совпадает с ним.

### <a name="filtering-on-schema-extension-properties-is-not-supported-on-all-entity-types"></a>Фильтрация по свойствам расширения схемы не поддерживается для всех типов объектов

Фильтрация по свойствам расширения схемы (с помощью выражения `$filter`) не поддерживается для типов объектов Outlook **contact**, **event**, **message** или **post**.

## <a name="files-onedrive"></a>Файлы (OneDrive)

### <a name="accessing-a-users-drive-before-user-accesses-it-leads-to-error"></a>Доступ к диску пользователя до того, как пользователь получит к нему доступ, приводит к ошибке

При первом доступе к личному диску пользователя с помощью Microsoft Graph до открытия им своего личного сайта в браузере возвращается ответ `401`.

## <a name="groups"></a>Группы

### <a name="admins-must-consent-to-permissions-for-groups-and-microsoft-teams"></a>Администраторы должны дать согласие на разрешения для групп и Microsoft Teams

Microsoft Graph предоставляет два разрешения ([*Group.Read.All*](permissions-reference.md#group-permissions) и [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) для доступа к API для групп и Microsoft Teams.
Эти разрешения должен предоставить администратор.
В будущем мы планируем добавить новые разрешения для групп и команд, которые смогут предоставлять пользователи.

### <a name="some-group-apis-dont-support-delegated-or-app-only-permissions"></a>Некоторые API группы не поддерживают делегирование разрешений только для приложений

Только API для базового администрирования групп и управления ими поддерживает доступ с помощью разрешений только для приложений или делегированных разрешений. Все остальные функции API групп поддерживают только делегированные разрешения.

Примеры функций групп, поддерживающих разрешения только для приложений и делегированные разрешения:

* создание и удаление групп;
* получение и обновление свойств групп, связанных с администрированием групп и управлением ими;
* синхронизация, типы и [параметры каталогов](/graph/api/resources/directoryobject) групп;
* владельцы и члены групп.
* Получение групповых бесед

Примеры функций групп, поддерживающих только делегированные разрешения:

* Групповые события, фотографии
* внешние отправители, разрешенные или запрещенные отправители, подписка на группы;
* избранное пользователей и счетчик непросмотренных элементов.

### <a name="microsoft-graph-bypasses-group-policies-configured-through-outlook-on-the-web"></a>Microsoft Graph обходит групповые политики, настроенные через Outlook в Интернете

Использование Microsoft Graph для создания группы Microsoft 365 и присвоения ей имени в обход всех групповых политик Microsoft 365, настроенных через Outlook в Интернете.

### <a name="allowexternalsenders-property-can-only-be-accessed-on-unified-groups"></a>Доступ к свойству allowExternalSenders можно получить только в объединенных группах

В настоящее время существует проблема, из-за которой невозможно установить свойство **allowExternalSenders** группы в операции POST или PATCH как в `/v1.0`, так и в `/beta`.

Доступ к свойству **allowExternalSenders** можно получить только в объединенных группах. Доступ к этому свойству в списках рассылки или группах безопасности, в том числе с помощью операций GET, приведет к ошибке.

### <a name="removing-a-group-owner-also-removes-the-user-as-a-group-member"></a>Удаление владельца группы также удаляет пользователя как участника группы

Если вызвать запрос [DELETE /groups/{id}/owners](/graph/api/group-delete-owners.md) для группы, связанной с [командой](/graph/api/resources/team.md), пользователь также удаляется из списка /groups/{id}/members. Чтобы устранить эту проблему, удалите пользователя из владельцев и участников, подождать 10 секунд и снова добавить его к участникам.

## <a name="identity-and-access"></a>Удостоверение и доступ

### <a name="conditional-access-policy-requires-consent-to-permission"></a>Политика условного доступа требует согласия на разрешение

API [conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy) в настоящее время требует согласия на разрешение **Policy.Read.All** для вызова методов POST и PATCH. В дальнейшем разрешение **Policy.ReadWrite.ConditionalAccess** позволит читать политики из каталога.

### <a name="claims-mapping-policy-might-require-consent-to-permissions"></a>Политика сопоставления утверждений может требовать согласия на разрешения

API [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy) может требовать согласия на разрешения **Policy.Read.All** и **Policy.ReadWrite.ConditionalAccess** для методов `LIST /policies/claimsMappingPolicies` и `GET /policies/claimsMappingPolicies/{id}` следующим образом:

+ Если в операции LIST нет объектов **claimsMappingPolicy** для получения, для вызова этого метода достаточно любого разрешения.
+ Если имеются объекты **claimsMappingPolicy** для получения, ваше приложение должно предоставить согласие на оба разрешения. Если они отсутствуют, ошибка `403 Forbidden` возвращается.

В будущем для вызова обоих методов будет достаточно любого разрешения.

## <a name="json-batching"></a>Пакетная обработка JSON

### <a name="nested-batches-are-not-supported"></a>Вложенные пакеты не поддерживаются

Пакетные запросы JSON не должны содержать вложенных пакетных запросов.

### <a name="all-individual-requests-must-be-synchronous"></a>Все отдельные запросы должны быть синхронными

Все запросы, содержащиеся в пакетном запросе, должны запускаться синхронно. Параметр `respond-async`, если он имеется, будет игнорироваться.

### <a name="transactional-processing-of-requests-is-not-supported"></a>Транзакция обработки запросов не поддерживается

В настоящее время Microsoft Graph не поддерживает диалоговую обработку отдельных запросов. Свойство **atomicityGroup** отдельных запросов будет игнорироваться.

### <a name="uris-must-be-relative"></a>URI должны быть относительными

Всегда указывайте относительные URI в пакетных запросах. Microsoft Graph сделает эти URL-адреса абсолютными с помощью конечной точки версии, включенной в URL-адрес пакета.

### <a name="batch-size-is-limited"></a>Размер пакета ограничен

В настоящее время в пакетный запрос JSON можно включить не более 20 отдельных запросов. 

* В зависимости от того, какие API-интерфейсы являются частью пакетного запроса, базовые службы налагают свои собственные ограничения регулирования, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.
* Запросы в пакете оцениваются индивидуально на предмет ограничений регулирования, и если какой-либо запрос превышает ограничения, он завершается ошибкой со статусом 429.

Дополнительные сведения см. в разделе [Регулирование и пакетная обработка](/graph/concepts/throttling.md#throttling-and-batching).

### <a name="request-dependencies-are-limited"></a>Зависимость запросов ограничена

Отдельные запросы могут зависеть от других отдельных запросов. В настоящее время запросы могут зависеть только от одного другого запроса и должны соответствовать одному из этих шаблонов:

- Параллельный — для отдельных запросов не указаны зависимости в свойстве **dependsOn**.
- Последовательный — все отдельные запросы зависят от предыдущего отдельного запроса.
- Идентичный — для всех отдельных запросов в свойстве **dependsOn** указана одна и та же зависимость. **Примечание**. Запросы, созданные с помощью этого шаблона, будут запускаться последовательно.

После усовершенствования пакетной обработки JSON эти ограничения будут удалены.

## <a name="mail-outlook"></a>Почта (Outlook)

### <a name="attaching-large-files-to-messages-with-delegated-permissions-can-fail"></a>Прикрепление больших файлов к сообщениям с делегированными разрешениями может привести к сбою
Приложение с делегированными разрешениями возвращает `HTTP 403 Forbidden` при попытке [присоединить большие файлы](outlook-large-attachments.md) к сообщению Outlook или событию, которое находится в общем или делегированном почтовом ящике. С делегированными разрешениями [createUploadSession](/graph/api/attachment-createuploadsession) завершается успешно, только если сообщение или событие находятся в почтовом ящике вошедшего в систему пользователя.

### <a name="the-comment-parameter-for-creating-a-draft-does-not-become-part-of-the-message-body"></a>Параметр comment для создания черновика не включается в текст сообщения

Параметр **comment** для создания ответа или черновика ([createReply](/graph/api/message-createreply), [createReplyAll](/graph/api/message-createreplyall), [createForward](/graph/api/message-createforward)) не включается в текст полученного черновика сообщения.

### <a name="get-messages-returns-chats-in-microsoft-teams"></a>При использовании запроса GET для сообщений возвращаются также чаты в Microsoft Teams

В конечных точках версии 1.0 и бета-версии данные отклика для `GET /users/id/messages` включают чаты Microsoft Teams, не входящие в область группы или канала. Тема этих сообщений чата: "IM".

## <a name="reports"></a>Отчеты

### <a name="azure-ad-activity-reports-can-return-an-error"></a>Отчеты о действиях Azure AD могут возвращать ошибку

Если у вас есть действительная лицензия Azure AD Premium и вы вызываете API отчетов о действиях Azure AD [directoryAudit](/graph/api/resources/directoryaudit), [signIn](/graph/api/resources/signin) или [provisioning](/graph/api/resources/provisioningobjectsummary), по-прежнему может возникнуть сообщение об ошибке, аналогичное указанному ниже.

```json
{
    "error": {
        "code": "Authentication_RequestFromNonPremiumTenantOrB2CTenant",
        "message": "Neither tenant is B2C or tenant doesn't have premium license",
        "innerError": {
            "date": "2021-09-02T17:15:30",
            "request-id": "73badd94-c0ca-4b09-a3e6-20c1f5f9a307",
            "client-request-id": "73badd94-c0ca-4b09-a3e6-20c1f5f9a307"
        }
    }
}
```
Эта ошибка также может возникнуть при получении свойства **signInActivity** ресурса [user](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true), например `https://graph.microsoft.com/beta/users?$select=signInActivity`.

Эта ошибка вызвана периодическими сбоями проверки лицензий. Мы работаем над их устранением. В качестве временного решения добавьте разрешение **Directory.Read.All**. Это временное решение не потребуется, когда проблема будет устранена.


## <a name="teamwork-microsoft-teams"></a>Работа в команде (Microsoft Teams)

### <a name="get-teams-is-not-supported"></a>GET / команды не поддерживается

Чтобы получить список команд, см. [список всех команд](teams-list-all-teams.md) и [список ваших команд](/graph/api/user-list-joinedteams).

### <a name="unable-to-filter-team-members-by-roles"></a>Не удается отфильтровать участников команды по ролям
Фильтры запросов ролей, а также другие фильтры `GET /teams/team-id/members?$filter=roles/any(r:r eq 'owner') and displayName eq 'dummy'` могут не работать. Сервер может вернуть `BAD REQUEST`.

### <a name="requests-to-filter-team-members-by-role-require-a-parameter"></a>В запросах на фильтрацию участников групп по ролям необходимо указывать один параметр

Во всех запросах на фильтрацию участников групп по ролям необходимо указывать либо параметр _skipToken_, либо параметр _top_, но не оба параметра одновременно. Если в запросе будут переданы оба параметра, параметр _top_ будет проигнорирован.

### <a name="some-properties-for-chat-members-might-be-missing-in-the-response-to-a-get-request"></a>Некоторые свойства для участников чата могут отсутствовать в ответе на запрос GET
В некоторых случаях свойство `tenantId` / `email` / `displayName` для отдельных участников чата может не заполняться в запросах `GET /chats/chat-id/members` или `GET /chats/chat-id/members/membership-id`.

### <a name="properties-are-missing-in-the-list-of-teams-that-a-user-has-joined"></a>В списке команд, к которым присоединился пользователь, отсутствуют свойства
Вызов API [me/joinedTeams](/graph/api/user-list-joinedteams) возвращает только свойства **id**, **displayName** и **description** [команды](/graph/api/resources/team). Чтобы получить все свойства, воспользуйтесь операцией [Получение команды](/graph/api/team-get).

### <a name="installation-of-apps-that-require-resource-specific-consent-permissions-is-not-supported"></a>Установка приложений, требующих разрешений на согласие для определенных ресурсов, не поддерживается
Следующие вызовы API не поддерживают установку приложений, требующих разрешений на [согласие для определенных ресурсов](https://aka.ms/teams-rsc).
- [Добавление приложения в команду](/graph/api/team-post-installedapps.md)
- [Обновление приложения, установленного в команде](/graph/api/team-teamsappinstallation-upgrade.md)
- [Добавление приложения в чат](/graph/api/chat-post-installedapps.md)
- [Обновление приложения, установленного в чате](/graph/api/chat-teamsappinstallation-upgrade.md)

## <a name="users"></a>Пользователи

### <a name="use-the-dollar--symbol-in-the-userprincipalname"></a>Использование символа доллара ($) в userPrincipalName

Microsoft Graph позволяет **userPrincipalName** начинать с символа доллара (`$`). Однако при запросе пользователей по userPrincipalName URL-адрес запроса `/users/$x@y.com` не выполняется. Это связано с тем, что этот URL-адрес запроса нарушает соглашение об URL-адресе OData, которые ожидают, что только параметры системного запроса будут иметь префикс символа `$`. В качестве обходного решения удалите косую черту (/) после `/users` и заключите **userPrincipalName** в скобки и одинарные кавычки следующим образом: `/users('$x@y.com')`.

### <a name="access-to-user-resources-is-delayed-after-creation"></a>Доступ к ресурсам пользователей задерживается после создания

Пользователей можно создавать мгновенно с помощью метода POST для объекта user. Для доступа к службам Microsoft 365 пользователю нужна соответствующая лицензия. Из-за распределенного характера службы файлы, сообщения и события этого пользователя станут доступны посредством API Microsoft Graph через 15 минут после назначения лицензии. В течение этого времени приложения будут получать ошибку HTTP `404`.

### <a name="access-to-a-users-profile-photo-is-limited"></a>Доступ к фотографии профиля пользователя ограничен

Просмотреть и обновить фотографию профиля пользователя можно, только если у пользователя есть почтовый ящик. Кроме того, все фотографии, которые, *возможно*, были сохранены с использованием свойства **thumbnailPhoto** (с помощью API Azure AD Graph [не рекомендуется] или путем синхронизации с AD Connect), больше недоступны с помощью свойства **photo** ресурса [user](/graph/api/resources/user) в Microsoft Graph.
Если в таком случае не удастся прочитать или изменить фотографию, возникнет следующая ошибка:

```javascript
{
  "error": {
    "code": "ErrorNonExistentMailbox",
    "message": "The SMTP address has no mailbox associated with it."
  }
}
```

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a>Отзыв сеансов входа возвращает неправильный код HTTP

[user: revokeSignInSessions API](/graph/api/user-revokesigninsessions) должен возвращать ответ `204 No content` в случае успешного отзыва и код ошибки HTTP (4xx или 5xx), если запрос не выполнен.    Однако из-за проблемы со службой этот API возвращает `200 OK` и логический параметр, который всегда `true`.  Пока проблема не будет устранена, любой код возврата 2xx можно интерпретировать как успешное выполнение запроса к этому API.

### <a name="incomplete-objects-are-returned-when-using-getbyids-request"></a>Неполные объекты возвращаются при использовании запроса getByIds

При запросе объектов с помощью [получения объектов каталога из списка идентификаторов](/graph/api/directoryobject-getbyids) должны возвращаться полные объекты. Однако в настоящее время объекты [user](/graph/api/resources/user) в конечной точке версии 1.0 возвращаются с ограниченным набором свойств. Временное решение: возврат более полных объектов [user](/graph/api/resources/user) обеспечивается при использовании операции в сочетании с параметром запроса `$select`. Это поведение не соответствует спецификациям OData. Так как это поведение может быть изменено в будущем, используйте это временное решение только при указании в параметре `$select=` всех нужных свойств и только если допускается внесение существенных изменений в это временное решение.

## <a name="query-parameters"></a>Параметры запроса 

### <a name="some-limitations-apply-to-query-parameters"></a>Некоторые ограничения применяются к параметрам запроса

К параметрам запроса применяются следующие ограничения:

* Не поддерживается несколько пространств имен.
* Не поддерживаются запросы GET для `$ref` и приведение для пользователей, групп, устройств, субъектов-служб и приложений.
* `@odata.bind` не поддерживается. Это означает, что вы не можете правильно настроить свойство навигации **acceptedSenders** или **rejectedSenders** в группе.
* Отсутствует `@odata.id` для навигации по объектам без вложений (например, сообщениям) при использовании минимальных метаданных.
* `$expand`:
  * Возвращает не более 20 объектов.
  * Отсутствует поддержка `@odata.nextLink`.
  * Поддерживается не более одного уровня развертывания.
  * Не поддерживаются дополнительные параметры (`$filter`, `$select`).
* `$filter`:
  * Конечная точка `/attachments` не поддерживает фильтры. При ее наличии параметр `$filter` игнорируется.
  * Фильтрация нескольких рабочих нагрузок не поддерживается.
* `$search`:
  * Полнотекстовый поиск доступен только для некоторых объектов, например сообщений.
  * Поиск по нескольким рабочим нагрузкам не поддерживается.
  * Поиск не поддерживается в клиентах Azure AD B2C.
* `$count`:
  * Не поддерживается в клиентах Azure AD B2C.
  * Если используется строка запроса `$count=true` во время запрашивания ресурсов каталога, свойство `@odata.count` будет присутствовать только на первой странице данных подкачки.
* Указанные в запросе параметры могут просто не сработать. Это может произойти, если не поддерживаются либо сами параметры, либо их сочетание.


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis-deprecated"></a>Функции, доступные только в REST API Office 365 или API Graph Azure AD (не рекомендуется)

Некоторые функции еще не доступны в Microsoft Graph. Если вы не нашли нужную функцию, можете использовать специальные [REST API Office 365](/previous-versions/office/office-365-api/). Сведения для Azure AD Graph см. в статье [Перенос приложений Azure Active Directory (Azure AD) Graph в Microsoft Graph](./migrate-azure-ad-graph-overview.md).
