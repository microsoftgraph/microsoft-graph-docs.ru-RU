---
title: Руководство по регулированию Microsoft Graph
description: Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 50b187209d722252e11df6a5cfc20ea5b796b875
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892781"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="96c16-105">Руководство по регулированию Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="96c16-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="96c16-p102">Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.</span><span class="sxs-lookup"><span data-stu-id="96c16-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="96c16-p103">Ограничения регулирования зависят от сценария. Например, при выполнении большого количества операций записи вероятность того, что понадобится регулирование, выше, чем при выполнении только операций чтения.</span><span class="sxs-lookup"><span data-stu-id="96c16-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="96c16-111">Что происходит при регулировании?</span><span class="sxs-lookup"><span data-stu-id="96c16-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="96c16-p104">При превышении порогового значения регулирования Microsoft Graph на некоторое время запрещает все последующие запросы от этого клиента. В случае регулирования Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), а запросы завершаются ошибкой. Рекомендуемое время ожидания возвращается в заголовке отклика на невыполненный запрос. Поведение регулирования зависит от типа и количества запросов. Например, при большом количестве запросов будут регулироваться запросы всех типов. Пороговые значения ограничений зависят от типа запроса. Могут возникать ситуации, в которых запросы на запись регулируются, а запросы на чтение разрешаются.</span><span class="sxs-lookup"><span data-stu-id="96c16-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="96c16-119">Распространенные сценарии регулирования</span><span class="sxs-lookup"><span data-stu-id="96c16-119">Common throttling scenarios</span></span>

<span data-ttu-id="96c16-120">Наиболее распространенные причины регулирования клиентов:</span><span class="sxs-lookup"><span data-stu-id="96c16-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="96c16-121">большое количество запросов во всех приложениях клиента;</span><span class="sxs-lookup"><span data-stu-id="96c16-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="96c16-122">большое количество запросов из конкретного приложения всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="96c16-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="96c16-123">Рекомендации по работе с регулированием</span><span class="sxs-lookup"><span data-stu-id="96c16-123">Best practices to handle throttling</span></span>

<span data-ttu-id="96c16-124">Ниже приведены рекомендации по работе с регулированием.</span><span class="sxs-lookup"><span data-stu-id="96c16-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="96c16-125">Сократите число операций каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="96c16-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="96c16-126">Сократите частоту вызовов.</span><span class="sxs-lookup"><span data-stu-id="96c16-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="96c16-127">Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.</span><span class="sxs-lookup"><span data-stu-id="96c16-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="96c16-p105">Во время реализации обработки ошибок можно обнаружить регулирование с помощью кода ошибки HTTP 429. Неудачный отклик содержит в заголовке поле `Retry-After`. Самый быстрый способ отключить регулирование — применить к запросам задержку `Retry-After`, так как Microsoft Graph продолжает регистрировать в журнале использование ресурсов при регулировании клиента.</span><span class="sxs-lookup"><span data-stu-id="96c16-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="96c16-131">Подождите столько секунд, сколько указано в заголовке `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="96c16-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="96c16-132">Повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="96c16-132">Retry the request.</span></span>
3. <span data-ttu-id="96c16-p106">Если запрос снова не удастся и будет получен код ошибки 429, регулирование продолжается. Используйте рекомендуемую задержку `Retry-After`, затем повторите запрос. Выполняйте эти действия, пока запрос не будет удачно выполнен.</span><span class="sxs-lookup"><span data-stu-id="96c16-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="96c16-135">Заголовок `Retry-After` сейчас доступен для ресурсов, представляющих следующее:</span><span class="sxs-lookup"><span data-stu-id="96c16-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="96c16-136">User</span><span class="sxs-lookup"><span data-stu-id="96c16-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- <span data-ttu-id="96c16-137">[фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="96c16-137">[Photo](/graph/api/resources/profilephoto?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="96c16-138">[почта](/graph/api/resources/message?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="96c16-138">[Mail](/graph/api/resources/message?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="96c16-139">[календарь (пользователи и группы)](/graph/api/resources/event?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="96c16-139">[Calendar (users and groups)](/graph/api/resources/event?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="96c16-140">[контакт](/graph/api/resources/contact?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="96c16-140">[Contact](/graph/api/resources/contact?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="96c16-141">[вложение](/graph/api/resources/attachment?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="96c16-141">[Attachment](/graph/api/resources/attachment?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="96c16-142">[групповые чаты](/graph/api/resources/conversation?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="96c16-142">[Group conversations](/graph/api/resources/conversation?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="96c16-143">[люди и социальные медиа](/graph/api/resources/social-overview?view=graph-rest-beta);</span><span class="sxs-lookup"><span data-stu-id="96c16-143">[People and social](/graph/api/resources/social-overview?view=graph-rest-beta)</span></span>
- <span data-ttu-id="96c16-144">[хранилище (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="96c16-144">[Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)</span></span>
- [<span data-ttu-id="96c16-145">внешний элемент (Поиск Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96c16-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)

<span data-ttu-id="96c16-146">Развернутое описание регулирования в Microsoft Cloud см. в [этой статье](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="96c16-146">For a broader discussion of throttling on the Microsoft Cloud, see [Throttling Pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="96c16-147">Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="96c16-147">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="96c16-148">Вы также можете реализовать [более сложные шаблоны](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.</span><span class="sxs-lookup"><span data-stu-id="96c16-148">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="96c16-149">В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="96c16-149">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="96c16-150">Ограничения для отдельных служб</span><span class="sxs-lookup"><span data-stu-id="96c16-150">Service-specific limits</span></span>

<span data-ttu-id="96c16-151">Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="96c16-151">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="96c16-152">В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="96c16-152">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="96c16-153">Описанные здесь отдельные ограничения могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="96c16-153">The specific limits described here are subject to change.</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="96c16-154">Ограничения службы Outlook</span><span class="sxs-lookup"><span data-stu-id="96c16-154">Outlook service limits</span></span>

<span data-ttu-id="96c16-155">Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="96c16-155">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="96c16-156">Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы).</span><span class="sxs-lookup"><span data-stu-id="96c16-156">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="96c16-157">Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="96c16-157">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span>

| <span data-ttu-id="96c16-158">Ограничение</span><span class="sxs-lookup"><span data-stu-id="96c16-158">Limit</span></span>                                                      | <span data-ttu-id="96c16-159">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="96c16-159">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="96c16-160">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="96c16-160">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="96c16-161">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="96c16-161">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="96c16-162">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="96c16-162">4 concurrent requests</span></span>                                      | <span data-ttu-id="96c16-163">Конечная точка бета-версии</span><span class="sxs-lookup"><span data-stu-id="96c16-163">Beta endpoint</span></span>   |
| <span data-ttu-id="96c16-164">Отправка 15 Мбит (PATCH, POST, PUT) в течение 30 секунд.</span><span class="sxs-lookup"><span data-stu-id="96c16-164">15 megabit upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="96c16-165">Конечная точка бета-версии</span><span class="sxs-lookup"><span data-stu-id="96c16-165">Beta endpoint</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="96c16-166">Ресурсы службы Outlook</span><span class="sxs-lookup"><span data-stu-id="96c16-166">Outlook service resources</span></span>

<span data-ttu-id="96c16-167">Службой Outlook представляются нижеперечисленные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="96c16-167">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="96c16-168">Ресурсы API календаря</span><span class="sxs-lookup"><span data-stu-id="96c16-168">Calendar API resources</span></span>

- [<span data-ttu-id="96c16-169">event</span><span class="sxs-lookup"><span data-stu-id="96c16-169">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="96c16-170">eventMessage</span><span class="sxs-lookup"><span data-stu-id="96c16-170">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="96c16-171">calendar</span><span class="sxs-lookup"><span data-stu-id="96c16-171">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="96c16-172">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="96c16-172">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="96c16-173">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="96c16-173">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="96c16-174">attachment</span><span class="sxs-lookup"><span data-stu-id="96c16-174">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="96c16-175">place (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="96c16-175">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="96c16-176">Ресурсы API почты</span><span class="sxs-lookup"><span data-stu-id="96c16-176">Mail API resources</span></span>

- [<span data-ttu-id="96c16-177">message</span><span class="sxs-lookup"><span data-stu-id="96c16-177">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="96c16-178">mailFolder</span><span class="sxs-lookup"><span data-stu-id="96c16-178">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="96c16-179">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="96c16-179">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="96c16-180">messageRule</span><span class="sxs-lookup"><span data-stu-id="96c16-180">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="96c16-181">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="96c16-181">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="96c16-182">attachment</span><span class="sxs-lookup"><span data-stu-id="96c16-182">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="96c16-183">Ресурсы API для управления личными контактами</span><span class="sxs-lookup"><span data-stu-id="96c16-183">Personal contacts API resources</span></span>

- [<span data-ttu-id="96c16-184">contact</span><span class="sxs-lookup"><span data-stu-id="96c16-184">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="96c16-185">contactFolder</span><span class="sxs-lookup"><span data-stu-id="96c16-185">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="96c16-186">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="96c16-186">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="96c16-187">Ресурсы социальной и рабочей аналитики</span><span class="sxs-lookup"><span data-stu-id="96c16-187">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="96c16-188">person</span><span class="sxs-lookup"><span data-stu-id="96c16-188">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="96c16-189">Ресурсы API задач из списка дел (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="96c16-189">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="96c16-190">outlookTask</span><span class="sxs-lookup"><span data-stu-id="96c16-190">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="96c16-191">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="96c16-191">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="96c16-192">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="96c16-192">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="96c16-193">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="96c16-193">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="96c16-194">attachment</span><span class="sxs-lookup"><span data-stu-id="96c16-194">attachment</span></span>](/graph/api/resources/attachment)
