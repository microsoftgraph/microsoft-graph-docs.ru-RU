---
title: Руководство по регулированию Microsoft Graph
description: Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: ef36b47b1666010dedf59d384742544ee35ceca5
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447109"
---
# <a name="microsoft-graph-throttling-guidance"></a>Руководство по регулированию Microsoft Graph

Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.

Ограничения регулирования зависят от сценария. Например, при выполнении большого количества операций записи вероятность того, что понадобится регулирование, выше, чем при выполнении только операций чтения.

> [!NOTE]
> Для решений, которым нужно извлекать большой объем данных из Microsoft Graph, вместо REST API Microsoft Graph должен использоваться [Microsoft Graph Data Connect](data-connect-concept-overview.md) . Microsoft Graph Data Connect позволяет организациям массово извлекать данные Microsoft 365 без ограничений регулирования.

<!-- markdownlint-disable MD033 -->
<br/>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a>Что происходит при регулировании?
<!-- markdownlint-enable MD026 -->

При превышении порогового значения регулирования Microsoft Graph на некоторое время запрещает все последующие запросы от этого клиента. В случае регулирования Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), а запросы завершаются ошибкой. Рекомендуемое время ожидания возвращается в заголовке отклика на невыполненный запрос. Поведение регулирования зависит от типа и количества запросов. Например, при большом количестве запросов будут регулироваться запросы всех типов. Пороговые значения ограничений зависят от типа запроса. Могут возникать ситуации, в которых запросы на запись регулируются, а запросы на чтение разрешаются.

## <a name="common-throttling-scenarios"></a>Распространенные сценарии регулирования

Наиболее распространенные причины регулирования клиентов:

- большое количество запросов во всех приложениях клиента;
- большое количество запросов из конкретного приложения всех клиентов.

## <a name="sample-response"></a>Пример отклика

При превышении порога регулирования Microsoft Graph реагирует с откликом, похожим на следующий.

```http
HTTP/1.1 429 Too Many Requests
Content-Type: application/json
Retry-After: 10

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

Во время реализации обработки ошибок можно обнаружить регулирование с помощью кода ошибки HTTP 429. Неудачный отклик содержит в заголовке поле `Retry-After`. Самый быстрый способ отключить регулирование — применить к запросам задержку `Retry-After`, так как Microsoft Graph продолжает регистрировать в журнале использование ресурсов при регулировании клиента.

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

Шаблоны программирования, такие как постоянные опросы на ресурсе для проверки обновлений и регулярное сканирование коллекций ресурсов для проверки наличия новых или удаленных ресурсов, чаще ведут к регулированию приложений и снижению общей производительности. Вместо этого следует использовать [отслеживание изменений](delta-query-overview.md) и [уведомления об изменениях](webhooks.md), когда они доступны.

>[!NOTE]
>Подробные сведения — в [рекомендациях по обнаружению файлов и определению изменений в масштабе](/onedrive/developer/rest-api/concepts/scan-guidance).

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

| API                                                      | Ресурсы      |
|------------------------------------------------------------|-----------------|
| API поиска (предварительная версия)                  | <li>[Внешний элемент (Поиск Майкрософт)](/graph/api/resources/externalitem) |
| API профиля                                      | <li>[Фотография](/graph/api/resources/profilephoto)   |
| API календаря | <li>[event](/graph/api/resources/event) <li> [eventMessage](/graph/api/resources/eventmessage) <li> [calendar](/graph/api/resources/calendar) <li>  [calendarGroup](/graph/api/resources/calendargroup) <li> [outlookCategory](/graph/api/resources/outlookcategory) <li> [attachment](/graph/api/resources/attachment) <li> [place (предварительный просмотр)](/graph/api/resources/place)   |
| API почты                                      | <li>[message](/graph/api/resources/message) <li>  [message](/graph/api/resources/message) <li> [mailFolder](/graph/api/resources/mailfolder) <li> [mailSearchFolder](/graph/api/resources/mailsearchfolder) <li> [messageRule](/graph/api/resources/messagerule) <li> [outlookCategory](/graph/api/resources/outlookcategory) <li> [attachment](/graph/api/resources/attachment)|
| API для управления личными контактами | <li>[contact](/graph/api/resources/contact) <li> [contactFolder](/graph/api/resources/contactfolder) <li> [outlookCategory](/graph/api/resources/outlookcategory)|
| Социальная и рабочая аналитика | <li>[person](/graph/api/resources/person) |
| API задач из списка дел (предварительная версия) | <li>[outlookTask](/graph/api/resources/outlooktask) <li> [outlookTaskFolder](/graph/api/resources/outlooktaskfolder) <li>[outlookTaskGroup](/graph/api/resources/outlooktaskgroup) <li> [outlookCategory](/graph/api/resources/outlookcategory) <li> [attachment](/graph/api/resources/attachment)|

### <a name="cloud-communication-service-limits"></a>Ограничения службы облачного взаимодействия

| Ресурс      | Ограничения для каждого приложения    |
| -------------- | ------------ |
| [Звонки](/graph/api/resources/call) | 10 000 звонков в месяц и 100 параллельных вызовов   |
| [Сведения о собрании](/graph/api/resources/meetinginfo)   | 2000 собраний на пользователя каждый месяц |
| [Присутствие](/graph/api/resources/presence)   | 1500 запросов в течение 30 секунд, на каждое приложение каждого клиента |

### <a name="onenote-service-limits"></a>Ограничения службы OneNote

| Тип ограничения | Ограничение по приложению на каждого пользователя (делегированный контекст) | Ограничение по приложению (контекст "только для приложений") |
| ------------ | ------- | ------- |
| Частота запросов | 120 запросов в 1 минуту и 400 запросов в 1 час | 240 запросов в 1 минуту и 800 запросов в 1 час |
| Параллельные запросы | 5 параллельных запросов | 20 параллельных запросов |

Указанные выше ограничения действуют для следующих ресурсов:

[!INCLUDE [Onenote throttling documentation](../includes/throttling-onenote.md)]

Дополнительные сведения о рекомендациях см. в статье [Регулирование в API OneNote и как его избежать](https://developer.microsoft.com/en-us/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).

**Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.

### <a name="project-rome-service-limits"></a>Ограничения службы Project Rome

| Тип запроса | Ограничение на каждого пользователя для всех приложений |
| ------------ | --------------------------- |
| GET          | 400 запросов в течение 5 минут и 12000 запросов в течение 1 дня |
| POST, PUT, PATCH, DELETE | 100 запросов в течение 5 минут и 8000 запросов в течение 1 дня |

Указанные выше ограничения действуют для следующих ресурсов:

- [activityHistoryItem](/graph/api/resources/activityhistoryitem)
- [userActivity](/graph/api/resources/useractivity)

### <a name="microsoft-teams-service-limits"></a>Ограничения службы Microsoft Teams

Ограничения выражаются в виде запросов в секунду (RPS).

| Тип запроса Teams                                   | Лимит на приложение на одного арендатора        | Ограничение на приложение для всех арендаторов      |
|------------------------------------------------------|---------------------------------|------------|
| ПОЛУЧИТЬ команду, канал, вкладку, установленные приложения, каталог приложений   | 30 запросов в секунду                          | 600 запросов в секунду |
| Канал POST / PUT, вкладка, установленные приложения, каталог приложений    |  30 запросов в секунду                         | 300 запросов в секунду  |
| PATCH команда, канал, вкладка, установленные приложения, каталог приложений |  30 запросов в секунду                         | 300 запросов в секунду  |
| УДАЛИТЬ канал, вкладку, установленные приложения, каталог приложений      |  15 запросов в секунду                         | 150 запросов в секунду  |
| Получить /teams/```{team-id}```, joinedTeams              |  30 запросов в секунду                         | 300 запросов в секунду  |
| POST /teams | 10 запросов в секунду | 100 запросов в секунду  |
| PUT /groups/```{team-id}```/team, клон | 6 запросов в секунду | 150 запросов в секунду  |
| ПОЛУЧИТЬ сообщение канала  | 20 запросов в секунду | 200 запросов в секунду |
| ПОЛУЧИТЬ 1: 1 / сообщение группового чата  | 20 запросов в секунду | 200 запросов в секунду |
| Сообщение POST канала | 50 запросов в секунду | 500 запросов в секунду |
| POST 1: 1 / сообщение в групповом чате | 20 запросов в секунду | 200 запросов в секунду |
| GET /teams/```{team-id}```/schedule и все API по этому пути | 30 запросов в секунду | 600 запросов в секунду |
| POST, PATCH, PUT /teams/```{team-id}```/schedule и все API по этому пути | 30 запросов в секунду | 300 запросов в секунду |
| DELETE /teams/```{team-id}```/schedule и все API по этому пути | 15 запросов в секунду | 150 запросов в секунду |
| POST /teams/```{team-id}```/sendActivityNotification | 5 запросов в секунду | 50 запросов в секунду |
| POST /chats/```{chat-id}```/sendActivityNotification | 5 запросов в секунду | 50 запросов в секунду |
| POST /users/```{user-id}```/teamwork/sendActivityNotification | 5 запросов в секунду | 50 запросов в секунду |
| Другие вызовы API GET для Microsoft Teams              | 30 запросов в секунду | 1500 запросов в секунду |
| Другие вызовы API для Microsoft Teams              | 30 запросов в секунду | 300 запросов в секунду |

Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.
Приложение может отправлять в определенный канал не более 3000 сообщений в день.

См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).

[!INCLUDE [Teams throttling documentation](../includes/throttling-teams.md)]

### <a name="identity-and-access-service-limits"></a>Ограничения службы удостоверения и доступа

Ограничения служб в этом разделе применяются к следующим объектам.

[!INCLUDE [Identity and access throttling documentation](../includes/throttling-identity-and-access.md)]

#### <a name="pattern"></a>Шаблон

Регулирование основано на алгоритме маркерной корзины, которая работает путем добавления отдельной стоимости запросов. Затем суммарная стоимость запросов сравнивается с заранее определенными ограничениями. Регулирование применяется только для запросов, превышающих ограничения. Если превышено любое из ограничений, будет получен отклик `429 Too Many Requests`. Отклики `429 Too Many Requests` можно получить даже в том случае, если следующие ограничения не достигнуты, когда службы находятся под важной нагрузкой или на основе объема данных для определенного клиента. В следующей таблице перечислены существующие ограничения.

| Тип ограничения | Квота единицы ресурса | Квота на запись |
| ---------- | ----------- | -------------- |
| пара "приложение + клиент" | S: 3 500 запросов за 10 секунд <br/> M: 5 000 запросов за 10 секунд <br/> L: 8 000 запросов за 10 секунд | 3 000 запросов за 2 минуты 30 секунд |
| приложение | 150 000 запросов за 20 секунд  | 70 000 запросов за 5 минут|
| клиент | Неприменимо | 18 000 запросов за 5 минут |

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

> [!IMPORTANT]
> 
> Стоимость операций POST, PATCH и DELETE в пути запроса `applications` зависит от типа **signInAudience**. Для приложений, для которых **signInAudience** относится к `AzureADMyOrg` или `AzureADMultipleOrgs`, стоимость составляет 70 000 запросов за 5 минут; а для приложений, для которых **signInAudience** относится к `AzureADandPersonalMicrosoftAccount` или `PersonalMicrosoftAccount`, стоимость составляет 60 запросов за минуту.

Другие факторы, влияющие на стоимость запросов:

- Использование `$select` снижает стоимость на 1
- Использование `$expand` увеличивает стоимость на 1
- Использование `$top` со значением меньше 20 снижает стоимость на 1
- Создание пользователя в клиенте Azure AD B2C увеличивает стоимость на 4

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

- **x-ms-throttle-scope** - eg. `Tenant_Application/ReadWrite/9a3d526c-b3c1-4479-ba74-197b5c5751ae/0785ef7c-2d7a-4542-b048-95bcab406e0b`. Указывает область регулирования в следующем формате `<Scope>/<Limit>/<ApplicationId>/<TenantId|UserId|ResourceId>`:
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

### <a name="identity-and-access-reports-service-limits"></a>Ограничения службы отчетов удостоверений и доступа

| Тип запроса |  Ограничение на приложение по клиенту |
| ------------ | ------------------------ |
| Любой | 5 запросов за 10 секунд |

Указанные выше ограничения действуют для следующих ресурсов:

[!INCLUDE [Azure AD identity and access reports throttling documentation](../includes/throttling-aad-reports.md)]

#### <a name="identity-and-access-reports-best-practices"></a>Рекомендации по отчетам об идентификации и доступе
API-интерфейсы отчетов Azure AD регулируются, когда Azure AD получает слишком много вызовов в течение заданного периода времени от клиента или приложения. Вызовы также могут быть ограничены, если служба отвечает слишком долго. Если ваши запросы по-прежнему завершаются ошибкой с кодом ошибки `429 Too Many Requests`, несмотря на применение [описанных выше рекомендаций](#best-practices-to-handle-throttling), попробуйте уменьшить объем возвращаемых данных. Сначала попробуйте эти подходы:
- Используйте фильтры, чтобы настроить запрос только на те данные, которые вам нужны. Если вам нужен только определенный тип события или подмножество пользователей, например, отфильтруйте другие события, используя параметры запроса `$filter` и `$select`, чтобы уменьшить размер объекта ответа и риск регулирования.
- Если вам нужен широкий набор данных отчетов Azure AD, используйте`$filter` для **createdDateTime**, чтобы ограничить количество событий входа, которые вы запрашиваете в одном вызове. Затем выполните итерацию по следующему промежутку времени, пока не получите все необходимые записи. Например, если вас регулируют, вы можете начать с вызова, запрашивающего данные за 3 дня, и выполнять итерации с более короткими промежутками времени, пока ваши запросы больше не будут регулироваться.
  
### <a name="information-protection-service-limits"></a>Ограничения службы защиты информации

Указанные ниже ограничения применяются к любому запросу в `/informationProtection`.

Для электронной почты ресурс — это уникальная пара ИД сетевого сообщения и получателя. Например, отправка письма с одним ИД сообщения одному пользователю несколько раз в течение 15 минут вызовет применение ограничения в соответствии с ограничениями для ресурсов, перечисленными в следующей таблице. Однако каждые 15 минут (ограничение клиента) можно отправлять до 150 уникальных писем.

| Операция                 | Ограничение для каждого клиента                                            | Ограничение на ресурс (электронная почта, URL-адрес, файл)                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| POST                      | 150 запросов в течение 15 минут и 10000 запросов в течение 24 часов | 1 запрос в течение 15 минут и 3 запроса в течение 24 часов |

[!INCLUDE [Information protection throttling documentation](../includes/throttling-information-protection.md)]

### <a name="identity-protection-and-conditional-access-service-limits"></a>Ограничения в отношении защиты удостоверений и службы условного доступа

| Тип запроса | Ограничение на клиента для всех приложений |
| ------------ | ------- |
| Любой | 1 запрос в секунду |

[!INCLUDE [Information protection throttling documentation](../includes/throttling-identityprotection-ca.md)]

> **Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.

### <a name="insights-service-limits"></a>Ограничения службы аналитики

Указанные ниже ограничения применяются к любому запросу в `me/insights` или `users/{id}/insights`.

| Ограничение                                                      | Сфера применения      |
|------------------------------------------------------------|-----------------|
| 10 000 запросов API в течение 10-минутного периода                  | Конечные точки версии 1.0 и бета-версии |
| 4 параллельных запроса                                      | Конечные точки версии 1.0 и бета-версии   |

Указанные выше ограничения действуют для следующих ресурсов:

- [people](/graph/api/resources/people)
- [sharedInsight](/graph/api/resources/sharedinsight)
- [trending](/graph/api/resources/trending)
- [usedInsight](/graph/api/resources/usedinsight)

### <a name="microsoft-graph-reports-service-limits"></a>Ограничения службы отчетов Microsoft Graph

Указанные ниже ограничения применяются к любому запросу в `/reports`.

| Операция                 | Ограничение на приложение по клиенту     | Ограничение на клиента для всех приложений |
|---------------------------|------------------------------|----------------------------|
| Любой запрос (CSV)         | 14 запросов в течение 10 минут   | 40 запросов в течение 10 минут |
| Любой запрос (JSON, beta)  | 100 запросов в течение 10 минут  | н/д                        |

Указанные выше ограничения применяются по отдельности к каждому API отчетов. Например, запрос к API отчетов о действиях пользователей Microsoft Teams и запрос к API отчетов о действиях пользователей Outlook в течение 10 минут будут рассматриваться как 1 запрос из 14 для каждого API, а не 2 запроса из 14 для обоих.

Указанные выше ограничения применяются к всем ресурсам [отчетов об использовании](/graph/api/resources/report).

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

Указанные выше ограничения действуют для следующих ресурсов:[!INCLUDE [Open and schema extensions throttling documentation](../includes/throttling-extensions.md)]

### <a name="files-and-lists-service-limits"></a>Ограничения службы для файлов и списков

Ограничения службы для OneDrive, OneDrive для бизнеса и SharePoint Online недоступны. Подробнее см. в статье [Почему нельзя просто назвать точные пределы регулирования?](/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online#why-cant-you-just-tell-me-the-exact-throttling-limits).

Сведения, приведенные в этой статье, относятся к следующим ресурсам:

[!INCLUDE [Files and lists throttling documentation](../includes/throttling-files-and-lists.md)]

### <a name="tasks-and-plans-service-limits"></a>Ограничения службы для задач и планов

Ограничения службы для Планировщика недоступны.

Сведения, указанные выше, относятся к следующим ресурсам: [!INCLUDE [Tasks and plans throttling documentation](../includes/throttling-tasks-and-plans.md)]

### <a name="identity-and-access-data-policy-operation-service-limits"></a>Ограничения службы операций с политикой данных удостоверений и доступа

| Тип запроса | Ограничение для каждого клиента |
| ------------ | ---------------- |
| POST для `exportPersonalData` | 1000 запросов в день по любой теме и 100 запросов по теме в день |
| Любой другой запрос | 10000 запросов в час |

Указанные выше ограничения действуют для следующих ресурсов:

- [dataPolicyOperation](/graph/api/resources/datapolicyoperation)

> **Примечание.** Перечисленные выше ресурсы не возвращают заголовок `Retry-After` в откликах `429 Too Many Requests`.

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a>Ограничения службы для образования

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a>Ограничения службы Excel

Объяснения и рекомендации, связанные с регулированием службы Excel, см. в статье [Уменьшение ошибок регулирования](workbook-best-practice.md#reduce-throttling-errors). Кроме того, ниже приведены некоторые ограничения регулирования.
  
[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-providers-service-limits"></a>Ограничения службы поставщиков удостоверений

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a>Ограничения службы Intune

[!INCLUDE [Intune  tunnel throttling documentation](../includes/throttling-intune-throttling-tunnel.md)]
[!INCLUDE [Intune android for work throttling documentation](../includes/throttling-intune-android-for-work.md)]
[!INCLUDE [Intune applications throttling documentation](../includes/throttling-intune-applications.md)]
[!INCLUDE [Intune auditing throttling documentation](../includes/throttling-intune-auditing.md)]
[!INCLUDE [Intune books throttling documentation](../includes/throttling-intune-books.md)]
[!INCLUDE [Intune bundles throttling documentation](../includes/throttling-intune-bundles.md)]
[!INCLUDE [Intune chromebook sync throttling documentation](../includes/throttling-intune-chromebook-sync.md)]
[!INCLUDE [Intune company terms throttling documentation](../includes/throttling-intune-company-terms.md)]
[!INCLUDE [Intune device config v2 throttling documentation](../includes/throttling-intune-device-config-v2.md)]
[!INCLUDE [Intune device configuration throttling documentation](../includes/throttling-intune-device-configuration.md)]
[!INCLUDE [Intune device enrollment throttling documentation](../includes/throttling-intune-device-enrollment.md)]
[!INCLUDE [Intune device intent throttling documentation](../includes/throttling-intune-device-intent.md)]
[!INCLUDE [Intune devices throttling documentation](../includes/throttling-intune-devices.md)]
[!INCLUDE [Intune endpoint protection throttling documentation](../includes/throttling-intune-endpoint-protection.md)]
[!INCLUDE [Intune enrollment throttling documentation](../includes/throttling-intune-enrollment.md)]
[!INCLUDE [Intune fencing throttling documentation](../includes/throttling-intune-fencing.md)]
[!INCLUDE [Intune GPAnalytics throttling documentation](../includes/throttling-intune-gpanalytics.md)]
[!INCLUDE [Intune managed applications throttling documentation](../includes/throttling-intune-managed-applications.md)]
[!INCLUDE [Intune notifications throttling documentation](../includes/throttling-intune-notifications.md)]
[!INCLUDE [Intune ODJ throttling documentation](../includes/throttling-intune-odj.md)]
[!INCLUDE [Intune partner integration throttling documentation](../includes/throttling-intune-partner-integration.md)]
[!INCLUDE [Intune rbac throttling documentation](../includes/throttling-intune-rbac.md)]
[!INCLUDE [Intune remote assistance throttling documentation](../includes/throttling-intune-remote-assistance.md)]
[!INCLUDE [Intune telephony throttling documentation](../includes/throttling-intune-telephony.md)]
[!INCLUDE [Intune TEM throttling documentation](../includes/throttling-intune-tem.md)]
[!INCLUDE [Intune troubleshooting throttling documentation](../includes/throttling-intune-troubleshooting.md)]
[!INCLUDE [Intune unlock throttling documentation](../includes/throttling-intune-unlock.md)]
[!INCLUDE [Intune updates throttling documentation](../includes/throttling-intune-updates.md)]
[!INCLUDE [Intune wip throttling documentation](../includes/throttling-intune-wip.md)]

### <a name="multi-service-limits"></a>Ограничения нескольких служб

[!INCLUDE [Multi tenant platform throttling documentation](../includes/throttling-multi-tenant-platform.md)]

### <a name="skype-service-limits"></a>Ограничения службы Skype

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a>Ограничения службы подписки

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->

### <a name="assignment-service-limits"></a>Ограничения службы заданий

Указанные ограничения применяются к запросам в API службы назначения.

| Тип запроса                 | Ограничение на приложение по клиенту     | Ограничение на клиента для всех приложений |
|---------------------------|------------------------------|----------------------------|
| Любой         | 500 запросов за 10 секунд   | 1000 запросов за 10 секунд
|Любой          | 15 000 запросов за 3600 секунд|30 000 запросов за 3600 секунд|
| GET me/задание  | 50 запросов за 10 секунд | 150 запросов за 10 секунд |

Указанные выше ограничения действуют для следующих ресурсов:

- [educationAssignment](/graph/api/resources/educationassignment)
- [educationSubmission](/graph/api/resources/educationsubmission)
- [trending](/graph/api/resources/trending)
- [educationResource](/graph/api/resources/educationresource)


### <a name="service-communications-service-limits"></a>Ограничения взаимодействия служб
Следующие ограничения применяются к любому типу запросов для взаимодействия служб в `/admin/serviceAnnouncement/`.

| Тип запроса |  Ограничение на приложение по клиенту |
| ------------ | ------------------------ |
| Любой | 240 запросов за 60 секунд |
|Любой | 800 запросов в час |

