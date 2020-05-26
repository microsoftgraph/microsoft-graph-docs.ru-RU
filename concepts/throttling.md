---
title: Руководство по регулированию Microsoft Graph
description: Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: d33ac4612f4fe3934c53235360626dac1393ab21
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44215789"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="37ba5-105">Руководство по регулированию Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="37ba5-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="37ba5-p102">Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.</span><span class="sxs-lookup"><span data-stu-id="37ba5-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="37ba5-p103">Ограничения регулирования зависят от сценария. Например, при выполнении большого количества операций записи вероятность того, что понадобится регулирование, выше, чем при выполнении только операций чтения.</span><span class="sxs-lookup"><span data-stu-id="37ba5-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="37ba5-111">Что происходит при регулировании?</span><span class="sxs-lookup"><span data-stu-id="37ba5-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="37ba5-p104">При превышении порогового значения регулирования Microsoft Graph на некоторое время запрещает все последующие запросы от этого клиента. В случае регулирования Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), а запросы завершаются ошибкой. Рекомендуемое время ожидания возвращается в заголовке отклика на невыполненный запрос. Поведение регулирования зависит от типа и количества запросов. Например, при большом количестве запросов будут регулироваться запросы всех типов. Пороговые значения ограничений зависят от типа запроса. Могут возникать ситуации, в которых запросы на запись регулируются, а запросы на чтение разрешаются.</span><span class="sxs-lookup"><span data-stu-id="37ba5-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="37ba5-119">Распространенные сценарии регулирования</span><span class="sxs-lookup"><span data-stu-id="37ba5-119">Common throttling scenarios</span></span>

<span data-ttu-id="37ba5-120">Наиболее распространенные причины регулирования клиентов:</span><span class="sxs-lookup"><span data-stu-id="37ba5-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="37ba5-121">большое количество запросов во всех приложениях клиента;</span><span class="sxs-lookup"><span data-stu-id="37ba5-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="37ba5-122">большое количество запросов из конкретного приложения всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="37ba5-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="37ba5-123">Рекомендации по работе с регулированием</span><span class="sxs-lookup"><span data-stu-id="37ba5-123">Best practices to handle throttling</span></span>

<span data-ttu-id="37ba5-124">Ниже приведены рекомендации по работе с регулированием.</span><span class="sxs-lookup"><span data-stu-id="37ba5-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="37ba5-125">Сократите число операций каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="37ba5-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="37ba5-126">Сократите частоту вызовов.</span><span class="sxs-lookup"><span data-stu-id="37ba5-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="37ba5-127">Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.</span><span class="sxs-lookup"><span data-stu-id="37ba5-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="37ba5-p105">Во время реализации обработки ошибок можно обнаружить регулирование с помощью кода ошибки HTTP 429. Неудачный отклик содержит в заголовке поле `Retry-After`. Самый быстрый способ отключить регулирование — применить к запросам задержку `Retry-After`, так как Microsoft Graph продолжает регистрировать в журнале использование ресурсов при регулировании клиента.</span><span class="sxs-lookup"><span data-stu-id="37ba5-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="37ba5-131">Подождите столько секунд, сколько указано в заголовке `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="37ba5-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="37ba5-132">Повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="37ba5-132">Retry the request.</span></span>
3. <span data-ttu-id="37ba5-p106">Если запрос снова не удастся и будет получен код ошибки 429, регулирование продолжается. Используйте рекомендуемую задержку `Retry-After`, затем повторите запрос. Выполняйте эти действия, пока запрос не будет удачно выполнен.</span><span class="sxs-lookup"><span data-stu-id="37ba5-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="37ba5-135">Заголовок `Retry-After` сейчас доступен для ресурсов, представляющих следующее:</span><span class="sxs-lookup"><span data-stu-id="37ba5-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="37ba5-136">User</span><span class="sxs-lookup"><span data-stu-id="37ba5-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- <span data-ttu-id="37ba5-137">[фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="37ba5-137">[Photo](/graph/api/resources/profilephoto?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="37ba5-138">[почта](/graph/api/resources/message?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="37ba5-138">[Mail](/graph/api/resources/message?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="37ba5-139">[календарь (пользователи и группы)](/graph/api/resources/event?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="37ba5-139">[Calendar (users and groups)](/graph/api/resources/event?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="37ba5-140">[контакт](/graph/api/resources/contact?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="37ba5-140">[Contact](/graph/api/resources/contact?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="37ba5-141">[вложение](/graph/api/resources/attachment?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="37ba5-141">[Attachment](/graph/api/resources/attachment?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="37ba5-142">[групповые чаты](/graph/api/resources/conversation?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="37ba5-142">[Group conversations](/graph/api/resources/conversation?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="37ba5-143">[люди и социальные медиа](/graph/api/resources/social-overview?view=graph-rest-beta);</span><span class="sxs-lookup"><span data-stu-id="37ba5-143">[People and social](/graph/api/resources/social-overview?view=graph-rest-beta)</span></span>
- <span data-ttu-id="37ba5-144">[хранилище (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="37ba5-144">[Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)</span></span>
- [<span data-ttu-id="37ba5-145">внешний элемент (Поиск Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37ba5-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)

<span data-ttu-id="37ba5-146">Развернутое описание регулирования в Microsoft Cloud см. в [этой статье](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="37ba5-146">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="37ba5-147">Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="37ba5-147">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="37ba5-148">Вы также можете реализовать [более сложные шаблоны](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.</span><span class="sxs-lookup"><span data-stu-id="37ba5-148">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="37ba5-149">В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="37ba5-149">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="37ba5-150">Рекомендации по избежанию регулирования</span><span class="sxs-lookup"><span data-stu-id="37ba5-150">Best practices to avoid throttling</span></span>

<span data-ttu-id="37ba5-151">Шаблоны программирования, например постоянные опросы на ресурсе для проверки обновлений и регулярное сканирование коллекций ресурсов для проверки новых или удаленных ресурсов, чаще ведут к регулированию приложений и ухудшению общей производительности.</span><span class="sxs-lookup"><span data-stu-id="37ba5-151">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="37ba5-152">Вместо этого необходимо по возможности использовать [отслеживание изменений](delta-query-overview.md) и [уведомления об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="37ba5-152">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="37ba5-153">Подробные сведения — в [рекомендациях по обнаружению файлов и определению изменений в масштабе](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).</span><span class="sxs-lookup"><span data-stu-id="37ba5-153">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="37ba5-154">Ограничения для отдельных служб</span><span class="sxs-lookup"><span data-stu-id="37ba5-154">Service-specific limits</span></span>

<span data-ttu-id="37ba5-155">Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="37ba5-155">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="37ba5-156">В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="37ba5-156">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="37ba5-157">Описанные здесь отдельные ограничения могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="37ba5-157">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="37ba5-158">Ограничения службы Outlook</span><span class="sxs-lookup"><span data-stu-id="37ba5-158">Outlook service limits</span></span>

<span data-ttu-id="37ba5-159">Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="37ba5-159">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="37ba5-160">Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы).</span><span class="sxs-lookup"><span data-stu-id="37ba5-160">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="37ba5-161">Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="37ba5-161">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span>

| <span data-ttu-id="37ba5-162">Ограничение</span><span class="sxs-lookup"><span data-stu-id="37ba5-162">Limit</span></span>                                                      | <span data-ttu-id="37ba5-163">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="37ba5-163">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="37ba5-164">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="37ba5-164">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="37ba5-165">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="37ba5-165">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="37ba5-166">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="37ba5-166">4 concurrent requests</span></span>                                      | <span data-ttu-id="37ba5-167">Конечная точка бета-версии</span><span class="sxs-lookup"><span data-stu-id="37ba5-167">Beta endpoint</span></span>   |
| <span data-ttu-id="37ba5-168">Отправка 15 Мбит (PATCH, POST, PUT) в течение 30 секунд.</span><span class="sxs-lookup"><span data-stu-id="37ba5-168">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="37ba5-169">Конечная точка бета-версии</span><span class="sxs-lookup"><span data-stu-id="37ba5-169">Beta endpoint</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="37ba5-170">Ресурсы службы Outlook</span><span class="sxs-lookup"><span data-stu-id="37ba5-170">Outlook service resources</span></span>

<span data-ttu-id="37ba5-171">Службой Outlook представляются нижеперечисленные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="37ba5-171">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="37ba5-172">Ресурсы API календаря</span><span class="sxs-lookup"><span data-stu-id="37ba5-172">Calendar API resources</span></span>

- [<span data-ttu-id="37ba5-173">event</span><span class="sxs-lookup"><span data-stu-id="37ba5-173">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="37ba5-174">eventMessage</span><span class="sxs-lookup"><span data-stu-id="37ba5-174">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="37ba5-175">calendar</span><span class="sxs-lookup"><span data-stu-id="37ba5-175">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="37ba5-176">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="37ba5-176">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="37ba5-177">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="37ba5-177">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="37ba5-178">attachment</span><span class="sxs-lookup"><span data-stu-id="37ba5-178">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="37ba5-179">place (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="37ba5-179">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="37ba5-180">Ресурсы API почты</span><span class="sxs-lookup"><span data-stu-id="37ba5-180">Mail API resources</span></span>

- [<span data-ttu-id="37ba5-181">message</span><span class="sxs-lookup"><span data-stu-id="37ba5-181">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="37ba5-182">mailFolder</span><span class="sxs-lookup"><span data-stu-id="37ba5-182">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="37ba5-183">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="37ba5-183">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="37ba5-184">messageRule</span><span class="sxs-lookup"><span data-stu-id="37ba5-184">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="37ba5-185">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="37ba5-185">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="37ba5-186">attachment</span><span class="sxs-lookup"><span data-stu-id="37ba5-186">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="37ba5-187">Ресурсы API для управления личными контактами</span><span class="sxs-lookup"><span data-stu-id="37ba5-187">Personal contacts API resources</span></span>

- [<span data-ttu-id="37ba5-188">contact</span><span class="sxs-lookup"><span data-stu-id="37ba5-188">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="37ba5-189">contactFolder</span><span class="sxs-lookup"><span data-stu-id="37ba5-189">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="37ba5-190">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="37ba5-190">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="37ba5-191">Ресурсы социальной и рабочей аналитики</span><span class="sxs-lookup"><span data-stu-id="37ba5-191">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="37ba5-192">person</span><span class="sxs-lookup"><span data-stu-id="37ba5-192">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="37ba5-193">Ресурсы API задач из списка дел (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="37ba5-193">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="37ba5-194">outlookTask</span><span class="sxs-lookup"><span data-stu-id="37ba5-194">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="37ba5-195">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="37ba5-195">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="37ba5-196">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="37ba5-196">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="37ba5-197">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="37ba5-197">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="37ba5-198">attachment</span><span class="sxs-lookup"><span data-stu-id="37ba5-198">attachment</span></span>](/graph/api/resources/attachment)

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="37ba5-199">Ограничения службы Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="37ba5-199">Microsoft Teams service limits</span></span>

<span data-ttu-id="37ba5-200">Ограничения выражаются в виде запросов в секунду (RPS).</span><span class="sxs-lookup"><span data-stu-id="37ba5-200">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="37ba5-201">Тип запроса Teams</span><span class="sxs-lookup"><span data-stu-id="37ba5-201">Teams request type</span></span>                                   | <span data-ttu-id="37ba5-202">Лимит на приложение на одного арендатора</span><span class="sxs-lookup"><span data-stu-id="37ba5-202">Limit per app per tenant</span></span>        | <span data-ttu-id="37ba5-203">Ограничение на приложение для всех арендаторов</span><span class="sxs-lookup"><span data-stu-id="37ba5-203">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="37ba5-204">Любой API Graph призывает Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="37ba5-204">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="37ba5-205">15000 запросов каждые 10 секунд</span><span class="sxs-lookup"><span data-stu-id="37ba5-205">15000 requests every 10 seconds</span></span> | <span data-ttu-id="37ba5-206">н/д</span><span class="sxs-lookup"><span data-stu-id="37ba5-206">n/a</span></span> |
| <span data-ttu-id="37ba5-207">ПОЛУЧИТЬ команду, канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="37ba5-207">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="37ba5-208">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-208">60 rps</span></span>                          | <span data-ttu-id="37ba5-209">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-209">600 rps</span></span> |
| <span data-ttu-id="37ba5-210">Канал POST / PUT, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="37ba5-210">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="37ba5-211">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-211">30 rps</span></span>                         | <span data-ttu-id="37ba5-212">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-212">300 rps</span></span>  |
| <span data-ttu-id="37ba5-213">PATCH команда, канал, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="37ba5-213">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="37ba5-214">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-214">30 rps</span></span>                         | <span data-ttu-id="37ba5-215">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-215">300 rps</span></span>  |
| <span data-ttu-id="37ba5-216">УДАЛИТЬ канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="37ba5-216">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="37ba5-217">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-217">15 rps</span></span>                         | <span data-ttu-id="37ba5-218">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-218">150 rps</span></span>  |
| <span data-ttu-id="37ba5-219">Получить /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="37ba5-219">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="37ba5-220">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-220">30 rps</span></span>                         | <span data-ttu-id="37ba5-221">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-221">300 rps</span></span>  |
| <span data-ttu-id="37ba5-222">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, клон</span><span class="sxs-lookup"><span data-stu-id="37ba5-222">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="37ba5-223">6 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-223">6 rps</span></span> | <span data-ttu-id="37ba5-224">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-224">150 rps</span></span>  | 
| <span data-ttu-id="37ba5-225">ПОЛУЧИТЬ сообщение канала</span><span class="sxs-lookup"><span data-stu-id="37ba5-225">GET channel message</span></span>  | <span data-ttu-id="37ba5-226">5 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-226">5 rps</span></span> | <span data-ttu-id="37ba5-227">100 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-227">100 rps</span></span> |
| <span data-ttu-id="37ba5-228">ПОЛУЧИТЬ 1: 1 / сообщение группового чата</span><span class="sxs-lookup"><span data-stu-id="37ba5-228">GET 1:1/group chat message</span></span>  | <span data-ttu-id="37ba5-229">3 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-229">3 rps</span></span> | <span data-ttu-id="37ba5-230">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-230">30 rps</span></span> |
| <span data-ttu-id="37ba5-231">Сообщение POST канала</span><span class="sxs-lookup"><span data-stu-id="37ba5-231">POST channel message</span></span> | <span data-ttu-id="37ba5-232">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-232">2 rps</span></span> | <span data-ttu-id="37ba5-233">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-233">20 rps</span></span> |
| <span data-ttu-id="37ba5-234">POST 1: 1 / сообщение в групповом чате</span><span class="sxs-lookup"><span data-stu-id="37ba5-234">POST 1:1/group chat message</span></span> | <span data-ttu-id="37ba5-235">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-235">2 rps</span></span> | <span data-ttu-id="37ba5-236">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="37ba5-236">20 rps</span></span> |

<span data-ttu-id="37ba5-237">Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.</span><span class="sxs-lookup"><span data-stu-id="37ba5-237">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="37ba5-238">Приложение может отправлять в определенный канал не более 3000 сообщений в день.</span><span class="sxs-lookup"><span data-stu-id="37ba5-238">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="37ba5-239">См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="37ba5-239">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="microsoft-graph-change-notifications-subscription-operations"></a><span data-ttu-id="37ba5-240">Операции подписки на уведомления об изменениях в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="37ba5-240">Microsoft Graph change notifications subscription operations</span></span>

<span data-ttu-id="37ba5-241">Указанные ниже ограничения применяются к любому запросу в `/subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="37ba5-241">The following limits apply to any request on `/subscriptions`.</span></span>

| <span data-ttu-id="37ba5-242">Операция</span><span class="sxs-lookup"><span data-stu-id="37ba5-242">Operation</span></span>                 | <span data-ttu-id="37ba5-243">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="37ba5-243">Limit per app per tenant</span></span>     | <span data-ttu-id="37ba5-244">Ограничение на приложение по всем клиентам</span><span class="sxs-lookup"><span data-stu-id="37ba5-244">Limit per app accross all tenants</span></span> |
|---------------------------|------------------------------|-----------------------------------|
| <span data-ttu-id="37ba5-245">POST, PUT, DELETE, PATCH</span><span class="sxs-lookup"><span data-stu-id="37ba5-245">POST, PUT, DELETE, PATCH</span></span>  | <span data-ttu-id="37ba5-246">1000 запросов за 20 секунд</span><span class="sxs-lookup"><span data-stu-id="37ba5-246">1000 requests per 20 seconds</span></span> | <span data-ttu-id="37ba5-247">2000 запросов за 20 секунд</span><span class="sxs-lookup"><span data-stu-id="37ba5-247">2000 requests per 20 seconds</span></span>      |
| <span data-ttu-id="37ba5-248">Все остальные методы HTTP</span><span class="sxs-lookup"><span data-stu-id="37ba5-248">All other HTTP methods</span></span>    | <span data-ttu-id="37ba5-249">5000 запросов за 20 секунд</span><span class="sxs-lookup"><span data-stu-id="37ba5-249">5000 requests per 20 seconds</span></span> | <span data-ttu-id="37ba5-250">10000 запросов за 20 секунд</span><span class="sxs-lookup"><span data-stu-id="37ba5-250">10000 requests per 20 seconds</span></span>     |
