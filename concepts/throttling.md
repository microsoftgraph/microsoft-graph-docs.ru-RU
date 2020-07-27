---
title: Руководство по регулированию Microsoft Graph
description: Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 8af7a4ce6c303e2ac07e4387ff3dbad38abd735e
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408094"
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

## <a name="best-practices-to-handle-throttling"></a>Рекомендации по работе с регулированием

Ниже приведены рекомендации по работе с регулированием.

- Сократите число операций каждого запроса.
- Сократите частоту вызовов.
- Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.

Во время реализации обработки ошибок можно обнаружить регулирование с помощью кода ошибки HTTP 429. Неудачный отклик содержит в заголовке поле `Retry-After`. Самый быстрый способ отключить регулирование — применить к запросам задержку `Retry-After`, так как Microsoft Graph продолжает регистрировать в журнале использование ресурсов при регулировании клиента.

1. Подождите столько секунд, сколько указано в заголовке `Retry-After`.
2. Повторите запрос.
3. Если запрос снова не удастся и будет получен код ошибки 429, регулирование продолжается. Используйте рекомендуемую задержку `Retry-After`, затем повторите запрос. Выполняйте эти действия, пока запрос не будет удачно выполнен.

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
- [Отчет](/graph/api/resources/report)
- [Подписка](/graph/api/resources/subscription)
- [Запрос на оценку угроз](/graph/api/resources/threatassessmentrequest)
- [Запрос на оценку почты](/graph/api/resources/mailassessmentrequest)
- [Запрос на оценку файла электронной почты](/graph/api/resources/emailfileassessmentrequest)
- [Запрос на оценку файла](/graph/api/resources/fileassessmentrequest)
- [Запрос на оценку URL-адреса](/graph/api/resources/urlassessmentrequest)
- [Результаты оценки угроз](/graph/api/resources/threatassessmentresult)
- [Популярное](/graph/api/resources/insights-trending)
- [Используемая аналитика](/graph/api/resources/insights-used)
- [Совместная аналитика](/graph/api/resources/insights-shared)
- [Параметры пользователя](/graph/api/resources/usersettings)
- [Приглашение](/graph/api/resources/invitation)

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

Любой запрос можно оценивать с учетом нескольких ограничений, в зависимости от области применения ограничения (для каждого приложения во всех клиентах, по клиенту для всех приложений, для каждого приложения по отдельному клиенту и т. д.), типа запроса (GET, POST, PATCH и т. д.) и других факторов. Первое достигнутое ограничение запускает действие регулирования. Помимо специальных ограничений для служб, описанных в этом разделе, применяются следующие глобальные ограничения:

| Тип запроса | Для каждого приложения во всех клиентах  |
| ------------ | ------------------------ |
| Любой          | 2000 запросов в секунду |

> [!NOTE]
> Описанные здесь отдельные ограничения могут изменяться.

> **Примечание.** В этом разделе термин *“клиент”* обозначает организацию Microsoft 365, в которой установлено приложение. Этот клиент может быть тем же самым, что и клиент, с которым создавалось приложение, в случае приложения с одним клиентом, или же он может отличаться в случае с [приложением, включающим несколько клиентов](/azure/active-directory/develop/setup-multi-tenant-app).

### <a name="outlook-service-limits"></a>Ограничения службы Outlook

Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика. Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы). Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику. Указанные ниже ограничения относятся к общедоступному облаку, а также к [национальным облачным развертываниям](/graph/deployments).

| Ограничение                                                      | Сфера применения      |
|------------------------------------------------------------|-----------------|
| 10 000 запросов API в течение 10-минутного периода                  | Конечные точки версии 1.0 и бета-версии |
| 4 параллельных запроса                                      | Конечные точки версии 1.0 и бета-версии   |
| Отправка 15 мегабайт (МБ) (PATCH, POST, PUT) в течение 30 секунд. | Конечные точки версии 1.0 и бета-версии   |

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

### <a name="cloud-communication-service-limits"></a>Ограничения службы облачного взаимодействия

| Ресурс      | Ограничения на приложение по клиенту    |
| -------------- | ------------ |
| [Звонки](/graph/api/resources/call) | 10 000 звонков в месяц и 100 параллельных вызовов   |
| [Сведения о собрании](/graph/api/resources/meetinginfo)   | 2000 собраний на пользователя каждый месяц |
| [Присутствие](/graph/api/resources/presence) (предварительная версия)   | 2 запроса в секунду |

### <a name="onenote-service-limits"></a>Ограничения службы OneNote

| Тип ограничения | Ограничение по приложению на каждого пользователя (делегированный контекст) | Ограничение по приложению (контекст "только для приложений") |
| ------------ | ------- | ------- |
| Частота запросов | 120 запросов в 1 минуту и 400 запросов в 1 час | 240 запросов в 1 минуту и 800 запросов в 1 час |
| Параллельные запросы | 5 параллельных запросов | 20 параллельных запросов |

Указанные выше ограничения действуют для следующих ресурсов:  
onenote, notebook, sectionGroup, onenoteSection, onenotePage, onenoteResource, onenoteOperation

Дополнительные сведения о рекомендациях см. в статье [Регулирование в API OneNote и как его избежать](https://developer.microsoft.com/ru-RU/office/blogs/onenote-api-throttling-and-how-to-avoid-it/).  

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

### <a name="microsoft-graph-reports-service-limits"></a>Ограничения службы отчетов Microsoft Graph

Указанные ниже ограничения применяются к любому запросу в `/reports`.

| Операция                 | Ограничение на приложение по клиенту     | Ограничение на клиента для всех приложений |
|---------------------------|------------------------------|----------------------------|
| Любой запрос (CSV)         | 14 запросов в течение 10 минут   | 40 запросов в течение 10 минут |
| Любой запрос (JSON, beta)  | 100 запросов в течение 10 минут  | н/д                        |

Указанные выше ограничения применяются по отдельности к каждому API отчетов. Например, запрос на API отчетов об активности пользователей Microsoft Teams и запрос на доступ к отчету об активности пользователей Outlook в течение 10 минут будут рассматриваться как 1 запрос из 14 для каждого API, а не 2 запроса из 14 для обоих.

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
