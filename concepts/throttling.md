---
title: Руководство по регулированию Microsoft Graph
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: f2acb34994f0877a051d31e276feb22b2d47179c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682042"
---
# <a name="microsoft-graph-throttling-guidance"></a>Руководство по регулированию Microsoft Graph

Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.

Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a>Что происходит при регулировании?
<!-- markdownlint-enable MD026 -->

When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.

## <a name="common-throttling-scenarios"></a>Распространенные сценарии регулирования

Наиболее распространенные причины регулирования клиентов:

- большое количество запросов во всех приложениях клиента;
- большое количество запросов из конкретного приложения всех клиентов.

## <a name="best-practices-to-handle-throttling"></a>Рекомендации по работе с регулированием

Ниже приведены рекомендации по работе с регулированием.

- Сократите число операций каждого запроса.
- Сократите частоту вызовов.
- Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.

When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.

1. Подождите столько секунд, сколько указано в заголовке `Retry-After`.
2. Повторите запрос.
3. If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.

Заголовок `Retry-After` сейчас доступен для ресурсов, представляющих следующее:

- [User](/graph/api/resources/user?view=graph-rest-1.0)
- [фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0);
- [почта](/graph/api/resources/message?view=graph-rest-1.0);
- [календарь (пользователи и группы)](/graph/api/resources/event?view=graph-rest-1.0);
- [контакт](/graph/api/resources/contact?view=graph-rest-1.0);
- [вложение](/graph/api/resources/attachment?view=graph-rest-1.0);
- [групповые чаты](/graph/api/resources/conversation?view=graph-rest-1.0);
- [люди и социальные медиа](/graph/api/resources/social-overview?view=graph-rest-beta);
- [хранилище (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0).
- [внешний элемент (Поиск Майкрософт)](/graph/api/resources/externalitem?view=graph-rest-beta)
- [Subscription](/graph/api/resources/subscription)

Развернутое описание регулирования в Microsoft Cloud см. в статье [Модель регулирования](https://docs.microsoft.com/azure/architecture/patterns/throttling).

> [!NOTE]
> Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки. Вы также можете реализовать [более сложные шаблоны](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.
>
> В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.

## <a name="best-practices-to-avoid-throttling"></a>Рекомендации по избежанию регулирования

Шаблоны программирования, например постоянные опросы на ресурсе для проверки обновлений и регулярное сканирование коллекций ресурсов для проверки новых или удаленных ресурсов, чаще ведут к регулированию приложений и ухудшению общей производительности. Вместо этого необходимо по возможности использовать [отслеживание изменений](delta-query-overview.md) и [уведомления об изменениях](webhooks.md).

>[!NOTE]
>Подробные сведения — в [рекомендациях по обнаружению файлов и определению изменений в масштабе](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).

## <a name="service-specific-limits"></a>Ограничения для отдельных служб

Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory. В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.

> [!NOTE]
> Описанные здесь отдельные ограничения могут изменяться.

### <a name="outlook-service-limits"></a>Ограничения службы Outlook

Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика. Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы). Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику.

| Ограничение                                                      | Сфера применения      |
|------------------------------------------------------------|-----------------|
| 10 000 запросов API в течение 10-минутного периода                  | Конечные точки версии 1.0 и бета-версии |
| 4 параллельных запроса                                      | Конечная точка бета-версии   |
| Отправка 15 Мбит (PATCH, POST, PUT) в течение 30 секунд. | Конечная точка бета-версии   |

#### <a name="outlook-service-resources"></a>Ресурсы службы Outlook

Службой Outlook представляются нижеперечисленные ресурсы.

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

Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.
Приложение может отправлять в определенный канал не более 3000 сообщений в день.

См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).

### <a name="microsoft-graph-change-notifications-subscription-operations"></a>Операции подписки на уведомления об изменениях в Microsoft Graph

Указанные ниже ограничения применяются к любому запросу в `/subscriptions`.

| Операция                 | Ограничение на приложение по клиенту     | Ограничение на приложение по всем клиентам |
|---------------------------|------------------------------|-----------------------------------|
| POST, PUT, DELETE, PATCH  | 1000 запросов за 20 секунд | 2000 запросов за 20 секунд      |
| Все остальные методы HTTP    | 5000 запросов за 20 секунд | 10000 запросов за 20 секунд     |
