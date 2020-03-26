---
title: Руководство по регулированию Microsoft Graph
description: Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: db87dfa7c855ba96b7cd7924b4f7829a6fd05a26
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962361"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="9e042-105">Руководство по регулированию Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9e042-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="9e042-p102">Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.</span><span class="sxs-lookup"><span data-stu-id="9e042-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="9e042-p103">Ограничения регулирования зависят от сценария. Например, при выполнении большого количества операций записи вероятность того, что понадобится регулирование, выше, чем при выполнении только операций чтения.</span><span class="sxs-lookup"><span data-stu-id="9e042-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="9e042-111">Что происходит при регулировании?</span><span class="sxs-lookup"><span data-stu-id="9e042-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="9e042-p104">При превышении порогового значения регулирования Microsoft Graph на некоторое время запрещает все последующие запросы от этого клиента. В случае регулирования Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), а запросы завершаются ошибкой. Рекомендуемое время ожидания возвращается в заголовке отклика на невыполненный запрос. Поведение регулирования зависит от типа и количества запросов. Например, при большом количестве запросов будут регулироваться запросы всех типов. Пороговые значения ограничений зависят от типа запроса. Могут возникать ситуации, в которых запросы на запись регулируются, а запросы на чтение разрешаются.</span><span class="sxs-lookup"><span data-stu-id="9e042-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="9e042-119">Распространенные сценарии регулирования</span><span class="sxs-lookup"><span data-stu-id="9e042-119">Common throttling scenarios</span></span>

<span data-ttu-id="9e042-120">Наиболее распространенные причины регулирования клиентов:</span><span class="sxs-lookup"><span data-stu-id="9e042-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="9e042-121">большое количество запросов во всех приложениях клиента;</span><span class="sxs-lookup"><span data-stu-id="9e042-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="9e042-122">большое количество запросов из конкретного приложения всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="9e042-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="9e042-123">Рекомендации по работе с регулированием</span><span class="sxs-lookup"><span data-stu-id="9e042-123">Best practices to handle throttling</span></span>

<span data-ttu-id="9e042-124">Ниже приведены рекомендации по работе с регулированием.</span><span class="sxs-lookup"><span data-stu-id="9e042-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="9e042-125">Сократите число операций каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="9e042-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="9e042-126">Сократите частоту вызовов.</span><span class="sxs-lookup"><span data-stu-id="9e042-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="9e042-127">Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.</span><span class="sxs-lookup"><span data-stu-id="9e042-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="9e042-p105">Во время реализации обработки ошибок можно обнаружить регулирование с помощью кода ошибки HTTP 429. Неудачный отклик содержит в заголовке поле `Retry-After`. Самый быстрый способ отключить регулирование — применить к запросам задержку `Retry-After`, так как Microsoft Graph продолжает регистрировать в журнале использование ресурсов при регулировании клиента.</span><span class="sxs-lookup"><span data-stu-id="9e042-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="9e042-131">Подождите столько секунд, сколько указано в заголовке `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="9e042-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="9e042-132">Повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="9e042-132">Retry the request.</span></span>
3. <span data-ttu-id="9e042-p106">Если запрос снова не удастся и будет получен код ошибки 429, регулирование продолжается. Используйте рекомендуемую задержку `Retry-After`, затем повторите запрос. Выполняйте эти действия, пока запрос не будет удачно выполнен.</span><span class="sxs-lookup"><span data-stu-id="9e042-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="9e042-135">Заголовок `Retry-After` сейчас доступен для ресурсов, представляющих следующее:</span><span class="sxs-lookup"><span data-stu-id="9e042-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="9e042-136">User</span><span class="sxs-lookup"><span data-stu-id="9e042-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- <span data-ttu-id="9e042-137">[фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="9e042-137">[Photo](/graph/api/resources/profilephoto?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="9e042-138">[почта](/graph/api/resources/message?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="9e042-138">[Mail](/graph/api/resources/message?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="9e042-139">[календарь (пользователи и группы)](/graph/api/resources/event?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="9e042-139">[Calendar (users and groups)](/graph/api/resources/event?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="9e042-140">[контакт](/graph/api/resources/contact?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="9e042-140">[Contact](/graph/api/resources/contact?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="9e042-141">[вложение](/graph/api/resources/attachment?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="9e042-141">[Attachment](/graph/api/resources/attachment?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="9e042-142">[групповые чаты](/graph/api/resources/conversation?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="9e042-142">[Group conversations](/graph/api/resources/conversation?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="9e042-143">[люди и социальные медиа](/graph/api/resources/social-overview?view=graph-rest-beta);</span><span class="sxs-lookup"><span data-stu-id="9e042-143">[People and social](/graph/api/resources/social-overview?view=graph-rest-beta)</span></span>
- <span data-ttu-id="9e042-144">[хранилище (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="9e042-144">[Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)</span></span>
- [<span data-ttu-id="9e042-145">внешний элемент (Поиск Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e042-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)

<span data-ttu-id="9e042-146">Развернутое описание регулирования в Microsoft Cloud см. в [этой статье](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="9e042-146">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="9e042-147">Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="9e042-147">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="9e042-148">Вы также можете реализовать [более сложные шаблоны](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.</span><span class="sxs-lookup"><span data-stu-id="9e042-148">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="9e042-149">В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="9e042-149">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="9e042-150">Ограничения для отдельных служб</span><span class="sxs-lookup"><span data-stu-id="9e042-150">Service-specific limits</span></span>

<span data-ttu-id="9e042-151">Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9e042-151">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="9e042-152">В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="9e042-152">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="9e042-153">Описанные здесь отдельные ограничения могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="9e042-153">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="9e042-154">Ограничения службы Outlook</span><span class="sxs-lookup"><span data-stu-id="9e042-154">Outlook service limits</span></span>

<span data-ttu-id="9e042-155">Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="9e042-155">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="9e042-156">Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы).</span><span class="sxs-lookup"><span data-stu-id="9e042-156">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="9e042-157">Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="9e042-157">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span>

| <span data-ttu-id="9e042-158">Ограничение</span><span class="sxs-lookup"><span data-stu-id="9e042-158">Limit</span></span>                                                      | <span data-ttu-id="9e042-159">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="9e042-159">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="9e042-160">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="9e042-160">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="9e042-161">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="9e042-161">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="9e042-162">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="9e042-162">4 concurrent requests</span></span>                                      | <span data-ttu-id="9e042-163">Конечная точка бета-версии</span><span class="sxs-lookup"><span data-stu-id="9e042-163">Beta endpoint</span></span>   |
| <span data-ttu-id="9e042-164">Отправка 15 Мбит (PATCH, POST, PUT) в течение 30 секунд.</span><span class="sxs-lookup"><span data-stu-id="9e042-164">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="9e042-165">Конечная точка бета-версии</span><span class="sxs-lookup"><span data-stu-id="9e042-165">Beta endpoint</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="9e042-166">Ресурсы службы Outlook</span><span class="sxs-lookup"><span data-stu-id="9e042-166">Outlook service resources</span></span>

<span data-ttu-id="9e042-167">Службой Outlook представляются нижеперечисленные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="9e042-167">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="9e042-168">Ресурсы API календаря</span><span class="sxs-lookup"><span data-stu-id="9e042-168">Calendar API resources</span></span>

- [<span data-ttu-id="9e042-169">event</span><span class="sxs-lookup"><span data-stu-id="9e042-169">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="9e042-170">eventMessage</span><span class="sxs-lookup"><span data-stu-id="9e042-170">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="9e042-171">calendar</span><span class="sxs-lookup"><span data-stu-id="9e042-171">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="9e042-172">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="9e042-172">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="9e042-173">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="9e042-173">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="9e042-174">attachment</span><span class="sxs-lookup"><span data-stu-id="9e042-174">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="9e042-175">place (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="9e042-175">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="9e042-176">Ресурсы API почты</span><span class="sxs-lookup"><span data-stu-id="9e042-176">Mail API resources</span></span>

- [<span data-ttu-id="9e042-177">message</span><span class="sxs-lookup"><span data-stu-id="9e042-177">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="9e042-178">mailFolder</span><span class="sxs-lookup"><span data-stu-id="9e042-178">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="9e042-179">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="9e042-179">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="9e042-180">messageRule</span><span class="sxs-lookup"><span data-stu-id="9e042-180">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="9e042-181">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="9e042-181">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="9e042-182">attachment</span><span class="sxs-lookup"><span data-stu-id="9e042-182">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="9e042-183">Ресурсы API для управления личными контактами</span><span class="sxs-lookup"><span data-stu-id="9e042-183">Personal contacts API resources</span></span>

- [<span data-ttu-id="9e042-184">contact</span><span class="sxs-lookup"><span data-stu-id="9e042-184">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="9e042-185">contactFolder</span><span class="sxs-lookup"><span data-stu-id="9e042-185">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="9e042-186">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="9e042-186">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="9e042-187">Ресурсы социальной и рабочей аналитики</span><span class="sxs-lookup"><span data-stu-id="9e042-187">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="9e042-188">person</span><span class="sxs-lookup"><span data-stu-id="9e042-188">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="9e042-189">Ресурсы API задач из списка дел (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="9e042-189">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="9e042-190">outlookTask</span><span class="sxs-lookup"><span data-stu-id="9e042-190">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="9e042-191">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9e042-191">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="9e042-192">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="9e042-192">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="9e042-193">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="9e042-193">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="9e042-194">attachment</span><span class="sxs-lookup"><span data-stu-id="9e042-194">attachment</span></span>](/graph/api/resources/attachment)

#### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="9e042-195">Ограничения службы Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9e042-195">Microsoft Teams service limits</span></span>

<span data-ttu-id="9e042-196">Ограничения выражаются в виде запросов в секунду (RPS).</span><span class="sxs-lookup"><span data-stu-id="9e042-196">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="9e042-197">Тип запроса Teams</span><span class="sxs-lookup"><span data-stu-id="9e042-197">Teams request type</span></span>                                   | <span data-ttu-id="9e042-198">Лимит на приложение на одного арендатора</span><span class="sxs-lookup"><span data-stu-id="9e042-198">Limit per app per tenant</span></span>        | <span data-ttu-id="9e042-199">Ограничение на приложение для всех арендаторов</span><span class="sxs-lookup"><span data-stu-id="9e042-199">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="9e042-200">Любой API Graph призывает Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9e042-200">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="9e042-201">15000 запросов каждые 10 секунд</span><span class="sxs-lookup"><span data-stu-id="9e042-201">15000 requests every 10 seconds</span></span> | <span data-ttu-id="9e042-202">н/д</span><span class="sxs-lookup"><span data-stu-id="9e042-202">n/a</span></span> |
| <span data-ttu-id="9e042-203">ПОЛУЧИТЬ команду, канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="9e042-203">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="9e042-204">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-204">60 rps</span></span>                          | <span data-ttu-id="9e042-205">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-205">600 rps</span></span> |
| <span data-ttu-id="9e042-206">Канал POST / PUT, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="9e042-206">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="9e042-207">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-207">30 rps</span></span>                         | <span data-ttu-id="9e042-208">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-208">300 rps</span></span>  |
| <span data-ttu-id="9e042-209">PATCH команда, канал, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="9e042-209">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="9e042-210">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-210">30 rps</span></span>                         | <span data-ttu-id="9e042-211">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-211">300 rps</span></span>  |
| <span data-ttu-id="9e042-212">УДАЛИТЬ канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="9e042-212">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="9e042-213">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-213">15 rps</span></span>                         | <span data-ttu-id="9e042-214">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-214">150 rps</span></span>  |
| <span data-ttu-id="9e042-215">Получить /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="9e042-215">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="9e042-216">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-216">30 rps</span></span>                         | <span data-ttu-id="9e042-217">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-217">300 rps</span></span>  |
| <span data-ttu-id="9e042-218">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, клон</span><span class="sxs-lookup"><span data-stu-id="9e042-218">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="9e042-219">6 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-219">6 rps</span></span> | <span data-ttu-id="9e042-220">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-220">150 rps</span></span>  | 
| <span data-ttu-id="9e042-221">ПОЛУЧИТЬ сообщение канала</span><span class="sxs-lookup"><span data-stu-id="9e042-221">GET channel message</span></span>  | <span data-ttu-id="9e042-222">5 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-222">5 rps</span></span> | <span data-ttu-id="9e042-223">100 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-223">100 rps</span></span> |
| <span data-ttu-id="9e042-224">ПОЛУЧИТЬ 1: 1 / сообщение группового чата</span><span class="sxs-lookup"><span data-stu-id="9e042-224">GET 1:1/group chat message</span></span>  | <span data-ttu-id="9e042-225">3 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-225">3 rps</span></span> | <span data-ttu-id="9e042-226">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-226">30 rps</span></span> |
| <span data-ttu-id="9e042-227">Сообщение POST канала</span><span class="sxs-lookup"><span data-stu-id="9e042-227">POST channel message</span></span> | <span data-ttu-id="9e042-228">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-228">2 rps</span></span> | <span data-ttu-id="9e042-229">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-229">20 rps</span></span> |
| <span data-ttu-id="9e042-230">POST 1: 1 / сообщение в групповом чате</span><span class="sxs-lookup"><span data-stu-id="9e042-230">POST 1:1/group chat message</span></span> | <span data-ttu-id="9e042-231">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-231">2 rps</span></span> | <span data-ttu-id="9e042-232">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="9e042-232">20 rps</span></span> |

<span data-ttu-id="9e042-233">Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.</span><span class="sxs-lookup"><span data-stu-id="9e042-233">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>

<span data-ttu-id="9e042-234">См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="9e042-234">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>