---
title: Руководство по регулированию Microsoft Graph
description: Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 88bbdf56f1ef59fe1e805437b34d46f7e8927613
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580986"
---
# <a name="microsoft-graph-throttling-guidance"></a>Руководство по регулированию Microsoft Graph

Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.

Ограничения регулирования зависят от сценария. Например, при выполнении большого количества операций записи вероятность того, что понадобится регулирование, выше, чем при выполнении только операций чтения.

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a>Что происходит при регулировании?
<!-- markdownlint-enable MD026 -->

При превышении порогового значения регулирования Microsoft Graph на некоторое время запрещает все последующие запросы от этого клиента. В случае регулирования Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), а запросы завершаются ошибкой. Рекомендуемое время ожидания возвращается в заголовке отклика на невыполненный запрос. Поведение регулирования зависит от типа и количества запросов. Например, при большом количестве запросов будут регулироваться запросы всех типов. Пороговые значения ограничений зависят от типа запроса. Могут возникать ситуации, в которых запросы на запись регулируются, а запросы на чтение разрешаются.

## <a name="common-throttling-scenarios"></a>Распространенные сценарии регулирования

Наиболее распространенные причины регулирования клиентов:

- большое количество запросов во всех приложениях клиента;
- большое количество запросов из конкретного приложения всех клиентов.

## <a name="sample-response"></a>Пример отклика

При превышении порога регулирования Microsoft Graph реагирует с откликом, похожим на следующий.

```http
HTTP/1.1 429 Too Many Requests
Content-Type: application/json
Retry-After: 2.128

{
  "error": {
    "code": "TooManyRequests",
    "innerError": {
      "code": "429",
      "date": "2020-08-18T12:51:51",
      "message": "Please retry after",
      "request-id": "94fb3b52-452a-4535-a601-69e0a90e3aa2",
      "status": "429"
    },
    "message": "Please retry again later."
  }
}
```

## <a name="best-practices-to-handle-throttling"></a>Рекомендации по решению проблем с регулированием

Ниже приведены рекомендации по работе с регулированием.

- Сократите число операций каждого запроса.
- Сократите частоту вызовов.
- Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.

Во время реализации обработки ошибок можно обнаружить регулирование с помощью кода ошибки HTTP 429. Неудачный отклик содержит в заголовке поле `Retry-After`. Самый быстрый способ отключить регулирование — применить к запросам задержку `Retry-After`, так как Microsoft Graph продолжает регистрировать в журнале использование ресурсов при регулировании клиента.

1. Подождите столько секунд, сколько указано в заголовке `Retry-After`.
2. Повторите запрос.
3. Если запрос снова не удастся и будет получен код ошибки 429, регулирование продолжается. Используйте рекомендуемую задержку `Retry-After`, затем повторите запрос. Выполняйте эти действия, пока запрос не будет удачно выполнен.

Все ресурсы и API, описанные в разделе [Ограничения для отдельных служб](#service-specific-limits), предоставляют заголовок `Retry-After`, если не указано иное.

Развернутое описание регулирования в Microsoft Cloud см. в статье [Модель регулирования](/azure/architecture/patterns/throttling).

> [!NOTE]
> Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки. Вы также можете реализовать [более сложные шаблоны](/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.
>
> В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.

## <a name="best-practices-to-avoid-throttling"></a>Рекомендации по избежанию регулирования

Шаблоны программирования, например постоянные опросы на ресурсе для проверки обновлений и регулярное сканирование коллекций ресурсов для проверки новых или удаленных ресурсов, чаще ведут к регулированию приложений и ухудшению общей производительности. Вместо этого необходимо по возможности использовать [отслеживание изменений](delta-query-overview.md) и [уведомления об изменениях](webhooks.md).

>[!NOTE]
>Подробные сведения — в [рекомендациях по обнаружению файлов и определению изменений в масштабе](/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).

## <a name="throttling-and-batching"></a>Регулирование и пакетная обработка

[Пакетная обработка JSON](./json-batching.md) позволяет оптимизировать приложение, объединив несколько запросов в один объект JSON. Запросы в пакете оцениваются отдельно по ограничениям регулирования, и если какой-либо запрос превышает ограничения, он не выполняется со значением `status` равным `429` и ошибкой, аналогичной указанной выше. Сам пакет не выполняется с кодом состояния `424` (ошибка зависимости). Возможно регулирование нескольких запросов в одном пакете. Вам следует повторно выполнить каждый неудачный запрос из пакета, используя значение, предоставленное в заголовке отклика `retry-after` из содержимого JSON. Вы можете повторить попытку выполнения всех неудачных запросов в новом пакете после самого долгого значения `retry-after`.

Если пакеты SDK автоматически повторно выполняют регулируемые запросы, не являющиеся пакетными, регулируемые запросы, входящие в пакет, не выполняются повторно автоматически.

## <a name="service-specific-limits"></a>Ограничения для отдельных служб

Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory. В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.

Любой запрос можно оценивать с учетом нескольких ограничений, в зависимости от области применения ограничения (для каждого приложения во всех клиентах, по клиенту для всех приложений, для каждого приложения по отдельному клиенту и т. д.), типа запроса (GET, POST, PATCH и т. д.) и других факторов. Первое достигнутое ограничение запускает действие регулирования. Помимо специальных ограничений для служб, описанных в этом разделе, применяются следующие глобальные ограничения:

| Тип запроса | Для каждого приложения во всех клиентах  |
| ------------ | ------------------------ |
| Любой          | 2000 запросов в секунду |

> [!NOTE]
> Описанные здесь отдельные ограничения могут изменяться.

> **Примечание.** В этом разделе термин *“клиент”* обозначает организацию Microsoft 365, в которой установлено приложение. Этот клиент может быть тем же самым, что и клиент, с которым создавалось приложение, в случае приложения с одним клиентом, или же он может отличаться в случае с [приложением, включающим несколько клиентов](/azure/active-directory/develop/setup-multi-tenant-app).

### <a name="outlook-service-limits"></a>Ограничения службы Outlook

Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика. Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы). Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику. Указанные ниже ограничения относятся к общедоступному облаку, а также к [национальным облачным развертываниям](./deployments.md).

| Ограничение                                                      | Сфера применения      |
|------------------------------------------------------------|-----------------|
| 10 000 запросов API в течение 10-минутного периода                  | Конечные точки версии 1.0 и бета-версии |
| 4 параллельных запроса                                      | Конечные точки версии 1.0 и бета-версии   |
| Отправка 15 мегабайт (МБ) (PATCH, POST, PUT) в течение 30 секунд. | Конечные точки версии 1.0 и бета-версии   |

#### <a name="outlook-service-resources"></a>Ресурсы службы Outlook

Службой Outlook представляются нижеперечисленные ресурсы.

##### <a name="search-api-resources-preview"></a>Ресурсы API поиска (предварительная версия)

- [Внешний элемент (Поиск Майкрософт)](/graph/api/resources/externalitem?view=graph-rest-beta)

##### <a name="profile-api-resources"></a>Ресурсы API профиля

- [Фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0)

##### <a name="calendar-api-resources"></a>Ресурсы API календаря

- [event](/graph/api/resources/event)
- [eventMessage](/graph/api/resources/eventmessage)
- [calendar](/graph/api/resources/calendar)
- [calendarGroup](/graph/api/resources/calendargroup)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)
- [place (предварительный просмотр)](/graph/api/resources/place)

##### <a name="mail-api-resources"></a>Ресурсы API почты

- [message](/graph/api/resources/message)
- [mailFolder](/graph/api/resources/mailfolder)
- [mailSearchFolder](/graph/api/resources/mailsearchfolder)
- [messageRule](/graph/api/resources/messagerule)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a>Ресурсы API для управления личными контактами

- [contact](/graph/api/resources/contact)
- [contactFolder](/graph/api/resources/contactfolder)
- [outlookCategory](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a>Ресурсы социальной и рабочей аналитики

- [person](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a>Ресурсы API задач из списка дел (предварительный просмотр)

- [outlookTask](/graph/api/resources/outlooktask)
- [outlookTaskFolder](/graph/api/resources/outlooktaskfolder)
- [outlookTaskGroup](/graph/api/resources/outlooktaskgroup)
- [outlookCategory](/graph/api/resources/outlookcategory)
- [attachment](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a>Ограничения службы облачного взаимодействия

| Ресурс      | Ограничения на приложение по клиенту    |
| -------------- | ------------ |
| [Звонки](/graph/api/resources/call) | 10 000 звонков в месяц и 100 параллельных вызовов   |
| [Сведения о собрании](/graph/api/resources/meetinginfo)   | 2000 собраний на пользователя каждый месяц |
| [Присутствие](/graph/api/resources/presence) (предварительная версия)   | 1500 запросов в течение 30 секунд, на каждое приложение каждого клиента |

### <a name="onenote-service-limits"></a>Ограничения службы OneNote

| Тип ограничения | Ограничение по приложению на каждого пользователя (делегированный контекст) | Ограничение по приложению (контекст "только для приложений") |
| ------------ | ------- | ------- |
| Частота запросов | 120 запросов в 1 минуту и 400 запросов в 1 час | 240 запросов в 1 минуту и 800 запросов в 1 час |
| Параллельные запросы | 5 параллельных запросов | 20 параллельных запросов |

Указанные выше ограничения действуют для следующих ресурсов:  
onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation

Дополнительные сведения о рекомендациях см. в статье [Регулирование в API OneNote и как его избежать](https://developer.microsoft.com/en-us/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).  

> **Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.

### <a name="project-rome-service-limits"></a>Ограничения службы Project Rome

| Тип запроса | Ограничение на каждого пользователя для всех приложений |
| ------------ | --------------------------- |
| GET          | 400 запросов в течение 5 минут и 12000 запросов в течение 1 дня |
| POST, PUT, PATCH, DELETE | 100 запросов в течение 5 минут и 8000 запросов в течение 1 дня |

Указанные выше ограничения действуют для следующих ресурсов:  
activityHistoryItem, userActivity

### <a name="microsoft-teams-service-limits"></a>Ограничения службы Microsoft Teams

Ограничения выражаются в виде запросов в секунду (RPS).

| Тип запроса Teams                                   | Лимит на приложение на одного арендатора        | Ограничение на приложение для всех арендаторов      |
|------------------------------------------------------|---------------------------------|------------|
| Любой API Graph призывает Microsoft Teams              | 15000 запросов каждые 10 секунд | н/д |
| ПОЛУЧИТЬ команду, канал, вкладку, установленные приложения, каталог приложений   | 60 запросов в секунду                          | 600 запросов в секунду |
| Канал POST / PUT, вкладка, установленные приложения, каталог приложений    |  30 запросов в секунду                         | 300 запросов в секунду  |
| PATCH команда, канал, вкладка, установленные приложения, каталог приложений |  30 запросов в секунду                         | 300 запросов в секунду  |
| УДАЛИТЬ канал, вкладку, установленные приложения, каталог приложений      |  15 запросов в секунду                         | 150 запросов в секунду  |
| Получить /teams/```{team-id}```, joinedTeams              |  30 запросов в секунду                         | 300 запросов в секунду  |
| POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, клон | 6 запросов в секунду | 150 запросов в секунду  |
| ПОЛУЧИТЬ сообщение канала  | 5 запросов в секунду | 100 запросов в секунду |
| ПОЛУЧИТЬ 1: 1 / сообщение группового чата  | 3 запроса в секунду | 30 запросов в секунду |
| Сообщение POST канала | 2 запроса в секунду | 20 запросов в секунду |
| POST 1: 1 / сообщение в групповом чате | 2 запроса в секунду | 20 запросов в секунду |
| GET /teams/```{team-id}```/schedule и все API по этому пути | 60 запросов в секунду | 600 запросов в секунду |
| POST, PATCH, PUT /teams/```{team-id}```/schedule и все API по этому пути | 30 запросов в секунду | 300 запросов в секунду |
| DELETE /teams/```{team-id}```/schedule и все API по этому пути | 15 запросов в секунду | 150 запросов в секунду |

Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.
Приложение может отправлять в определенный канал не более 3000 сообщений в день.

См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).

Указанные выше ограничения действуют для следующих ресурсов:  
aadUserConversationMember, appCatalogs, changeTrackedEntity, channel, chatMessage, chatMessageHostedContent, conversationMember, offerShiftRequest, openShift, openShiftChangeRequest, schedule, scheduleChangeRequest, schedulingGroup, shift, shiftPreferences, swapShiftsChangeRequest, team, teamsApp, teamsAppDefinition, teamsAppInstallation, teamsAsyncOperation, teamsTab, teamsTemplate, teamwork, timeOff, timeOffReason, timeOffRequest, userSettings, workforceIntegration.

### <a name="identity-and-access-service-limits"></a>Ограничения службы удостоверения и доступа

Эти ограничения службы действуют для следующих объектов:

- [Объект каталога](/graph/api/resources/directoryobject)
- [Свойство расширения](/graph/api/resources/extensionproperty)
- [Административная единица](/graph/api/resources/administrativeunit)
- [Приложение](/graph/api/resources/application)
- [Назначение ролей приложения](/graph/api/resources/approleassignment)
- [Настройка проверки подлинности на основе сертификата](/graph/api/resources/certificatebasedauthconfiguration)
- [Контакты организации](/graph/api/resources/orgcontact)
- [Устройство](/graph/api/resources/device)
- [Ссылка партнера на объект каталога](/graph/api/resources/directoryobjectpartnerreference)
- [Роль каталога](/graph/api/resources/directoryrole)
- [Шаблон для ролей каталога](/graph/api/resources/directoryroletemplate)
- [Домен](/graph/api/resources/domain)
- [DNS-запись домена](/graph/api/resources/domaindnsrecord)
- [DNS-запись CNAME домена](/graph/api/resources/domaindnscnamerecord)
- [DNS-запись MX домена](/graph/api/resources/domaindnsmxrecord)
- [DNS-запись SRV домена](/graph/api/resources/domaindnssrvrecord)
- [DNS-запись TXT домена](/graph/api/resources/domaindnstxtrecord)
- [Недоступная запись DNS домена](/graph/api/resources/domaindnsunavailablerecord)
- [Конечная точка](/graph/api/resources/endpoint)
- [Свойство расширения](/graph/api/resources/extensionproperty)
- [Сведения о лицензии](/graph/api/resources/licensedetails)
- [Группа](/graph/api/resources/group)
- [Политика времени ожидания на основании активности](/graph/api/resources/activitybasedtimeoutpolicy)
- [Политика сопоставления утверждений](/graph/api/resources/claimsmappingpolicy)
- [Политика обнаружения домашней области](/graph/api/resources/homerealmdiscoverypolicy)
- [Политика выпуска маркеров](/graph/api/resources/tokenissuancepolicy)
- [Политика времени существования маркера](/graph/api/resources/tokenlifetimepolicy)
- [Основа политики](/graph/api/resources/policybase)
- [Политика STS](/graph/api/resources/stspolicy)
- [Соглашение](/graph/api/resources/contract)
- [Субъект-служба](/graph/api/resources/serviceprincipal)
- [Подписанная единица SKU](/graph/api/resources/subscribedsku)
- [Предоставление разрешения OAuth2](/graph/api/resources/oauth2permissiongrant)
- [Организация](/graph/api/resources/organization)
- [Пользователь](/graph/api/resources/user)
- [Параметр группы](/graph/api/resources/groupsetting)
- [Шаблон параметров группы](/graph/api/resources/groupsettingtemplate)

#### <a name="pattern"></a>Шаблон

Регулирование основано на алгоритме маркерной корзины, которая работает путем добавления отдельной стоимости запросов. Затем суммарная стоимость запросов сравнивается с заранее определенными ограничениями. Регулирование применяется только для запросов, превышающих ограничения. Если превышено любое из ограничений, будет получен отклик `429 Too Many Requests`. Отклики `429 Too Many Requests` можно получить даже в том случае, если следующие ограничения не достигнуты, когда службы находятся под важной нагрузкой или на основе объема данных для определенного клиента. В следующей таблице перечислены существующие ограничения.

| Тип ограничения | Квота единицы ресурса | Квота на запись |
| ---------- | ----------- | -------------- |
| пара "приложение + клиент" | S: 3500, M: 5000, L: 8000 за 10 секунд | 3000 за 2 минуты 30 секунд |
| приложение | 150 000 за 20 секунд  | 70 000 за 5 минут |
| клиент | Неприменимо | 18 000 за 5 минут |

> **Примечание**. Ограничение пары "приложение + клиент" зависит от количества пользователей в клиенте, в котором выполняются запросы. Размеры клиента определяются следующим образом: S — менее 50 пользователей, M — от 50 до 500 пользователей и L — более 500 пользователей.

В следующей таблице перечислены базовые стоимости запросов. У любых запросов, не указанных в списке, базовая стоимость равна 1.

| Операция | Путь запроса | Базовая стоимость единицы ресурса | Стоимость записи |
| --------- | ------------ | ----------------- | ------------------ |
| GET | `applications` | 2 | 0 |
| GET | `applications/{id}/extensionProperties` | 2 | 0 |
| GET | `contracts` | 3 | 0 |
| POST | `directoryObjects/getByIds` |  3 | 0 |
| GET | `domains/{id}/domainNameReferences` | 4 | 0 |
| POST | `getObjectsById` | 3 | 0 |
| GET | `groups/{id}/members` | 3 | 0 |
| GET | `groups/{id}/transitiveMembers` | 5 | 0 |
| POST | `isMemberOf` | 4 | 0 |
| POST | `me/checkMemberGroups` | 4 | 0 |
| POST | `me/checkMemberObjects` | 4 | 0 |
| POST | `me/getMemberGroups` | 2 | 0 |
| POST | `me/getMemberObjects` | 2 | 0 |
| GET | `me/licenseDetails` | 2 | 0 |
| GET | `me/memberOf` | 2 | 0 |
| GET | `me/ownedObjects` | 2 | 0 |
| GET | `me/transitiveMemberOf` | 2 | 0 |
| GET | `oauth2PermissionGrants` | 2 | 0 |
| GET | `oauth2PermissionGrants/{id}` | 2 | 0 |
| GET | `servicePrincipals/{id}/appRoleAssignments` | 2 | 0 |
| GET | `subscribedSkus` | 3 | 0 |
| GET | `users` | 2 | 0 |
| GET | Любой путь удостоверения, не указанный в таблице | 1 | 0 |
| POST | Любой путь удостоверения, не указанный в таблице | 1 | 1 |
| PATCH | Любой путь удостоверения, не указанный в таблице | 1 | 1 |
| PUT | Любой путь удостоверения, не указанный в таблице | 1 | 1 |
| DELETE | Любой путь удостоверения, не указанный в таблице | 1 | 1 |

Другие факторы, влияющие на стоимость запросов:

- Использование `$select` снижает стоимость на 1
- Использование `$expand` увеличивает стоимость на 1
- Использование `$top` со значением меньше 20 снижает стоимость на 1

> **Примечание**. Стоимость запроса никогда не может быть меньше 1. Любая стоимость запроса, применяемая к пути запроса, начинающегося с `me/`, также применяется к аналогичным запросам, начинающимся с `users/{id | userPrincipalName}/`.

#### <a name="additional-headers"></a>Дополнительные заголовки

##### <a name="request-headers"></a>Заголовки запросов

- **x-ms-throttle-priority**. Если заголовок не существует или для него задано другое значение, это означает, что это нормальный запрос. Рекомендуем присваивать приоритету значение `high` только для запросов, инициированных пользователем. Этот заголовок может иметь следующие значения:
  - Low. Означает низкий приоритет запроса. Регулирование этого запроса не вызывает заметные для пользователя сбои.
  - Normal. Применяется по умолчанию, если значение не указано. Означает стандартный приоритет запроса.
  - High. Означает высокий приоритет запроса. Регулирование этого запроса вызывает заметные для пользователя сбои.

> **Примечание.** Если требуется регулирование запросов, запросы с низким приоритетом будут регулироваться первыми, с нормальным приоритетом — вторыми, а с высоким приоритетом — последними. Использование заголовка запроса с приоритетом не изменяет ограничения.

##### <a name="regular-responses-requests"></a>Обычные запросы откликов

- **x-ms-resource-unit**. Указывает единицу ресурса, примененную для запроса. Значения: положительные целые числа.
- **x-ms-throttle-limit-percentage**. Возвращается только в том случае, если приложение израсходовало более 0,8 от ограничения. Значения в диапазоне от 0,8 до 1,8, соответствующие проценту использования ограничения. Значение может использоваться вызывающими для настройки оповещений и выполнения действий.

##### <a name="throttled-responses-requests"></a>Регулируемые запросы откликов

- **x-ms-throttle-scope**. Например: `Tenant_Application/ReadWrite/9a3d526c-b3c1-4479-ba74-197b5c5751ae/0785ef7c-2d7a-4542-b048-95bcab406e0b`. Указывает область регулирования в следующем формате — `<Scope>/<Limit>/<ApplicationId>/<TenantId|UserId|ResourceId>`:
  - Scope: (строка, обязательно)
    - Tenant_Application — все запросы определенного клиента для текущего приложения.
    - Tenant — все запросы для текущего клиента независимо от приложения.
    - Application — все запросы для текущего приложения.
  - Limit: (строка, обязательно)
    - Read. Запросы на чтение в области (GET)
    - Write. Запросы на запись в области (POST, PATCH, PUT, DELETE...)
    - ReadWrite. Все запросы в области (любые)
  - ApplicationId (GUID, обязательно)
  - TenantId|UserId|ResourceId: (GUID, обязательно)
- **x-ms-throttle-information**. Указывает причину регулирования и может иметь любое значение (строка). Это значение предоставляется для диагностики и устранения неполадок. Вот несколько примеров:
  - CPULimitExceeded — регулирование вызвано превышением ограничения для выделения ЦП.
  - WriteLimitExceeded — регулирование вызвано превышением ограничения на запись.
  - ResourceUnitLimitExceeded — регулирование вызвано превышением ограничения для выделенного ресурса.

### <a name="information-protection"></a>Защита информации

Указанные ниже ограничения применяются к любому запросу в `/informationProtection`.

| Операция                 | Ограничение для каждого клиента                                            | Ограничение на ресурс (электронная почта, URL-адрес, файл)                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| POST                      | 150 запросов в течение 15 минут и 10000 запросов в течение 24 часов | 1 запрос в течение 15 минут и 3 запроса в течение 24 часов |

Указанные выше ограничения действуют для следующих ресурсов:  
threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.

### <a name="identity-protection-and-conditional-access-service-limits"></a>Ограничения в отношении защиты удостоверений и службы условного доступа

| Тип запроса | Ограничение на клиента для всех приложений |
| ------------ | ------- |
| Любой | 1 запрос в секунду |

Указанные выше ограничения действуют для следующих ресурсов:  
riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.

> **Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.

### <a name="insights-service-limits"></a>Ограничения службы аналитики

Указанные ниже ограничения применяются к любому запросу в `me/insights` или `users/{id}/insights`.

| Ограничение                                                      | Сфера применения      |
|------------------------------------------------------------|-----------------|
| 10 000 запросов API в течение 10-минутного периода                  | Конечные точки версии 1.0 и бета-версии |
| 4 параллельных запроса                                      | Конечные точки версии 1.0 и бета-версии   |

Указанные выше ограничения действуют для следующих ресурсов:  
people, trending, usedinsight, sharedInsight.

### <a name="microsoft-graph-reports-service-limits"></a>Ограничения службы отчетов Microsoft Graph

Указанные ниже ограничения применяются к любому запросу в `/reports`.

| Операция                 | Ограничение на приложение по клиенту     | Ограничение на клиента для всех приложений |
|---------------------------|------------------------------|----------------------------|
| Любой запрос (CSV)         | 14 запросов в течение 10 минут   | 40 запросов в течение 10 минут |
| Любой запрос (JSON, beta)  | 100 запросов в течение 10 минут  | н/д                        |

Указанные выше ограничения применяются по отдельности к каждому API отчетов. Например, запрос к API отчетов об активности пользователей Microsoft Teams и запрос к API отчетов об активности пользователей Outlook в течение 10 минут будут рассматриваться как 1 запрос из 14 для каждого API, а не 2 запроса из 14 для обоих.

Указанные выше ограничения применяются для ресурса **report**.  

### <a name="invitation-manager-service-limits"></a>Ограничения службы диспетчера приглашений

Указанные ниже ограничения применяются к любому запросу в `/invitations`.

| Операция                 | Ограничение на клиента для всех приложений |
|---------------------------|------------------------------|
| Любая операция             | 150 запросов за 5 секунд   |

### <a name="security-detections-and-incidents-service-limits"></a>Ограничения службы обнаружений и инцидентов безопасности

Указанные ниже ограничения применяются к любому запросу в `/security`.

| Операция                  | Ограничение на приложение по клиенту     |
|----------------------------|------------------------------|
| Любые операции с `alert`, `securityActions`  `secureScore` | 150 запросов в минуту      |
| Любая операция с `tiIndicator` | 1000 запросов в минуту |
| Любая операция с `secureScore` или `secureScorecontrolProfile` | 10 000 запросов API в течение 10-минутного периода |
| Любая операция с `secureScore` или `secureScorecontrolProfile` | 4 параллельных запроса |

### <a name="open-and-schema-extensions-service-limits"></a>Ограничения службы для открытых расширений и расширений схемы

| Тип запроса | Ограничение на приложение по клиенту |
| ------------ | ------------------------ |
| Любой          | 455 запросов в течение 10 секунд |

Указанные выше ограничения действуют для следующих ресурсов: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post и user.

### <a name="files-and-lists-service-limits"></a>Ограничения службы для файлов и списков

Ограничения службы для OneDrive, OneDrive для бизнеса и SharePoint Online недоступны. Подробнее см. в статье [Почему нельзя просто назвать точные пределы регулирования?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).

Сведения, приведенные в этой статье, относятся к следующим ресурсам:  
baseItem, baseItemVersion, columnDefinition, columnLink, contentType, drive, driveItem, driveItemVersion, fieldValueSet, itemActivity, itemActivityStat, itemAnalytics, list, listItem, listItemVersion, permission, sharedDriveItem, site и thumbnailSet.

### <a name="tasks-and-plans-service-limits"></a>Ограничения службы для задач и планов

Ограничения службы для Планировщика недоступны.

Сведения, приведенные в этой статье, относятся к следующим ресурсам:  
planner, plannerAssignedToTaskBoardTaskFormat, plannerBucket, plannerBucketTaskBoardTaskFormat, plannerGroup, plannerPlan, plannerPlanDetails, plannerProgressTaskBoardTaskFormat, plannerTask, plannerTaskDetails и plannerUser.

### <a name="identity-and-access-data-policy-operation-service-limits"></a>Ограничения службы операций с политикой данных удостоверений и доступа

| Тип запроса | Ограничение для каждого клиента |
| ------------ | ---------------- |
| POST для `exportPersonalData` | 1000 запросов в день по любой теме и 100 запросов по теме в день |
| Любой другой запрос | 10000 запросов в час |

Указанные выше ограничения действуют для следующих ресурсов: dataPolicyOperation.

> **Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a>Ограничения службы для образования

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a>Ограничения службы Excel

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a>Ограничения службы журналов аудита удостоверения и доступа

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a>Ограничения службы поставщиков удостоверений

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a>Ограничения службы Intune

[!INCLUDE [Intune applications throttling documentation](../includes/throttling-intune-applications.md)]
[!INCLUDE [Intune books throttling documentation](../includes/throttling-intune-books.md)]
[!INCLUDE [Intune company terms throttling documentation](../includes/throttling-intune-company-terms.md)]
[!INCLUDE [Intune device configuration throttling documentation](../includes/throttling-intune-device-configuration.md)]
[!INCLUDE [Intune device enrollment throttling documentation](../includes/throttling-intune-device-enrollment.md)]
[!INCLUDE [Intune devices throttling documentation](../includes/throttling-intune-devices.md)]
[!INCLUDE [Intune enrollment throttling documentation](../includes/throttling-intune-enrollment.md)]
[!INCLUDE [Intune managed applications throttling documentation](../includes/throttling-intune-managed-applications.md)]
[!INCLUDE [Intune notifications throttling documentation](../includes/throttling-intune-notifications.md)]
[!INCLUDE [Intune rbac throttling documentation](../includes/throttling-intune-rbac.md)]
[!INCLUDE [Intune remote assistance throttling documentation](../includes/throttling-intune-remote-assistance.md)]
[!INCLUDE [Intune reporting throttling documentation](../includes/throttling-intune-reporting.md)]
[!INCLUDE [Intune TEM throttling documentation](../includes/throttling-intune-tem.md)]
[!INCLUDE [Intune troubleshooting throttling documentation](../includes/throttling-intune-troubleshooting.md)]
[!INCLUDE [Intune wip throttling documentation](../includes/throttling-intune-wip.md)]

### <a name="skype-service-limits"></a>Ограничения службы Skype

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a>Ограничения службы подписки

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->

### <a name="assignment-service-limits"></a>Ограничения службы заданий

Указанные ограничения применяются к запросам в API бета-версии службы назначения.

| Тип запроса                 | Ограничение на приложение по клиенту     | Ограничение на клиента для всех приложений |
|---------------------------|------------------------------|----------------------------|
| Любой         | 5000 запросов в течение 10 секунд   | 15 000 запросов за 10 секунд |
| GET me/задание  | 50 запросов за 10 секунд | 150 запросов за 10 секунд |  

Предыдущие ограничения действуют для следующих ресурсов: [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta)
[educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta)
[educationResource](/graph/api/resources/educationresource?view=graph-rest-beta)
