---
title: Руководство по регулированию Microsoft Graph
description: Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 5561e8a28440f05adcd074b6cd7d4d61edbb2852
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050787"
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
- [Report](/graph/api/resources/report)
- [Subscription](/graph/api/resources/subscription)
- [Популярные](/graph/api/resources/insights-trending)
- [Использованная аналитика](/graph/api/resources/insights-used)
- [Общая информация](/graph/api/resources/insights-shared)
- [Параметры пользователя](/graph/api/resources/usersettings)
- [Отправлен](/graph/api/resources/invitation)

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

> **Примечание:** В этом разделе термин " *клиент* " относится к организации Microsoft 365, в которой установлено приложение. Это может быть тот же клиент, что и в том случае, когда приложение было создано, в случае одного клиентского приложения, или оно может отличаться в случае [приложения с несколькими клиентами](/azure/active-directory/develop/setup-multi-tenant-app).

### <a name="outlook-service-limits"></a>Ограничения службы Outlook

Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика. Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы). Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику. Следующие пределы применяются к общедоступному облаку, а также к [облачным облачным развертываниям](/graph/deployments).

| Ограничение                                                      | Сфера применения      |
|------------------------------------------------------------|-----------------|
| 10 000 запросов API в течение 10-минутного периода                  | Конечные точки версии 1.0 и бета-версии |
| 4 параллельных запроса                                      | Конечные точки версии 1.0 и бета-версии   |
| Загрузка 15 мегабайт (МБ) (исправление, POST, PUT) за 30-секундный период | Конечные точки версии 1.0 и бета-версии   |

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

### <a name="cloud-communication-service-limits"></a>Пределы облачных служб связи

| Ресурс      | Максимальное число приложений для каждого клиента    |
| -------------- | ------------ |
| [Звонки](/graph/api/resources/call) | 10 000 звонков/мес и 100 одновременные вызовы   |
| [Сведения о собрании](/graph/api/resources/meetinginfo)   | 2000 собраний и пользователей в месяц |
| [Присутствие](/graph/api/resources/presence) (Предварительная версия)   | 2 запроса в секунду |

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
| ПОЛУЧЕНИЕ/Teams/ ```{team-id}``` /счедуле и всех API по этому пути | 60 запросов в секунду | 600 запросов в секунду |
| POST, PATCH, PUT/Teams/ ```{team-id}``` /счедуле и все API по этому пути | 30 запросов в секунду | 300 запросов в секунду |
| Удалите/Teams/ ```{team-id}``` /счедуле и все API, расположенные по этому пути | 15 запросов в секунду | 150 запросов в секунду |

Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.
Приложение может отправлять в определенный канал не более 3000 сообщений в день.

См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).

### <a name="insights-service-limits"></a>Пределы службы аналитики

Следующие пределы применяются к запросам на `me/insights` или `users/{id}/insights` .

| Ограничение                                                      | Сфера применения      |
|------------------------------------------------------------|-----------------|
| 10 000 запросов API в течение 10-минутного периода                  | Конечные точки версии 1.0 и бета-версии |
| 4 параллельных запроса                                      | Конечные точки версии 1.0 и бета-версии   |

### <a name="microsoft-graph-reports-service-limits"></a>Пределы службы отчетов Microsoft Graph

Указанные ниже ограничения применяются к любому запросу в `/reports`.

| Операция                 | Ограничение на приложение по клиенту     | Максимальное количество для каждого клиента           |
|---------------------------|------------------------------|----------------------------|
| Любой запрос (CSV)         | 14 запросов в течение 10 минут   | 40 запросов в течение 10 минут |
| Любой запрос (JSON, бета-версия)  | 100 запросов в течение 10 минут  | н/д                        |

Предыдущие пределы применяются по отдельности к каждому API отчетов. Например, запрос к API отчетов об активности пользователей Microsoft Teams и запрос на отчеты об активности пользователей в Outlook в течение 10 минут будут считаться 1 запросом из 14 для каждого API, а не 2 запросами из 14.

### <a name="invitation-manager-service-limits"></a>Пределы службы диспетчера приглашений

Указанные ниже ограничения применяются к любому запросу в `/invitations`.

| Операция                 | Максимальное количество для каждого клиента             |
|---------------------------|------------------------------|
| Любая операция             | 150 запросов в течение 5 секунд   |

<!-- { "blockType": "throttlinggenstart" } -->

### <a name="education-service-limits"></a>Пределы службы образования

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a>Пределы для служб Excel

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a>Пределы службы журналов аудита удостоверений и доступа

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a>Пределы службы поставщиков удостоверений

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a>Пределы службы Intune

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

### <a name="skype-service-limits"></a>Пределы для служб Skype

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a>Пределы для службы подписки

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
