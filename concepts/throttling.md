---
title: Руководство по регулированию Microsoft Graph
description: Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 96592654fffb3111a398178d807da702c398e0d2
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165116"
---
# <a name="microsoft-graph-throttling-guidance"></a><span data-ttu-id="123fd-105">Руководство по регулированию Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="123fd-105">Microsoft Graph throttling guidance</span></span>

<span data-ttu-id="123fd-p102">Регулирование позволяет ограничить количество одновременных вызовов службы, чтобы предотвратить перегрузку ресурсов. Служба Microsoft Graph предназначена для обработки большого количества запросов. Регулирование помогает поддерживать оптимальную производительность и надежность службы Microsoft Graph, если выполняется слишком много запросов.</span><span class="sxs-lookup"><span data-stu-id="123fd-p102">Throttling limits the number of concurrent calls to a service to prevent overuse of resources. Microsoft Graph is designed to handle a high volume of requests. If an overwhelming number of requests occurs, throttling helps maintain optimal performance and reliability of the Microsoft Graph service.</span></span>

<span data-ttu-id="123fd-p103">Ограничения регулирования зависят от сценария. Например, при выполнении большого количества операций записи вероятность того, что понадобится регулирование, выше, чем при выполнении только операций чтения.</span><span class="sxs-lookup"><span data-stu-id="123fd-p103">Throttling limits vary based on the scenario. For example, if you are performing a large volume of writes, the possibility for throttling is higher than if you are only performing reads.</span></span>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a><span data-ttu-id="123fd-111">Что происходит при регулировании?</span><span class="sxs-lookup"><span data-stu-id="123fd-111">What happens when throttling occurs?</span></span>
<!-- markdownlint-enable MD026 -->

<span data-ttu-id="123fd-p104">При превышении порогового значения регулирования Microsoft Graph на некоторое время запрещает все последующие запросы от этого клиента. В случае регулирования Microsoft Graph возвращает код состояния HTTP 429 (слишком много запросов), а запросы завершаются ошибкой. Рекомендуемое время ожидания возвращается в заголовке отклика на невыполненный запрос. Поведение регулирования зависит от типа и количества запросов. Например, при большом количестве запросов будут регулироваться запросы всех типов. Пороговые значения ограничений зависят от типа запроса. Могут возникать ситуации, в которых запросы на запись регулируются, а запросы на чтение разрешаются.</span><span class="sxs-lookup"><span data-stu-id="123fd-p104">When a throttling threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>

## <a name="common-throttling-scenarios"></a><span data-ttu-id="123fd-119">Распространенные сценарии регулирования</span><span class="sxs-lookup"><span data-stu-id="123fd-119">Common throttling scenarios</span></span>

<span data-ttu-id="123fd-120">Наиболее распространенные причины регулирования клиентов:</span><span class="sxs-lookup"><span data-stu-id="123fd-120">The most common causes of throttling of clients include:</span></span>

- <span data-ttu-id="123fd-121">большое количество запросов во всех приложениях клиента;</span><span class="sxs-lookup"><span data-stu-id="123fd-121">A large number of requests across all applications in a tenant.</span></span>
- <span data-ttu-id="123fd-122">большое количество запросов из конкретного приложения всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="123fd-122">A large number of requests from a particular application across all tenants.</span></span>

## <a name="best-practices-to-handle-throttling"></a><span data-ttu-id="123fd-123">Рекомендации по работе с регулированием</span><span class="sxs-lookup"><span data-stu-id="123fd-123">Best practices to handle throttling</span></span>

<span data-ttu-id="123fd-124">Ниже приведены рекомендации по работе с регулированием.</span><span class="sxs-lookup"><span data-stu-id="123fd-124">The following are best practices for handling throttling:</span></span>

- <span data-ttu-id="123fd-125">Сократите число операций каждого запроса.</span><span class="sxs-lookup"><span data-stu-id="123fd-125">Reduce the number of operations per request.</span></span>
- <span data-ttu-id="123fd-126">Сократите частоту вызовов.</span><span class="sxs-lookup"><span data-stu-id="123fd-126">Reduce the frequency of calls.</span></span>
- <span data-ttu-id="123fd-127">Избегайте немедленных повторов, так как запросы накапливаются, и их количество превышает ограничения использования.</span><span class="sxs-lookup"><span data-stu-id="123fd-127">Avoid immediate retries, because all requests accrue against your usage limits.</span></span>

<span data-ttu-id="123fd-p105">Во время реализации обработки ошибок можно обнаружить регулирование с помощью кода ошибки HTTP 429. Неудачный отклик содержит в заголовке поле `Retry-After`. Самый быстрый способ отключить регулирование — применить к запросам задержку `Retry-After`, так как Microsoft Graph продолжает регистрировать в журнале использование ресурсов при регулировании клиента.</span><span class="sxs-lookup"><span data-stu-id="123fd-p105">When you implement error handling, use the HTTP error code 429 to detect throttling. The failed response includes the `Retry-After` response header. Backing off requests using the `Retry-After` delay is the fastest way to recover from throttling because Microsoft Graph continues to log resource usage while a client is being throttled.</span></span>

1. <span data-ttu-id="123fd-131">Подождите столько секунд, сколько указано в заголовке `Retry-After`.</span><span class="sxs-lookup"><span data-stu-id="123fd-131">Wait the number of seconds specified in the `Retry-After` header.</span></span>
2. <span data-ttu-id="123fd-132">Повторите запрос.</span><span class="sxs-lookup"><span data-stu-id="123fd-132">Retry the request.</span></span>
3. <span data-ttu-id="123fd-p106">Если запрос снова не удастся и будет получен код ошибки 429, регулирование продолжается. Используйте рекомендуемую задержку `Retry-After`, затем повторите запрос. Выполняйте эти действия, пока запрос не будет удачно выполнен.</span><span class="sxs-lookup"><span data-stu-id="123fd-p106">If the request fails again with a 429 error code, you are still being throttled. Continue to use the recommended `Retry-After` delay and retry the request until it succeeds.</span></span>

<span data-ttu-id="123fd-135">Заголовок `Retry-After` сейчас доступен для ресурсов, представляющих следующее:</span><span class="sxs-lookup"><span data-stu-id="123fd-135">The following resources currently provide a `Retry-After` header:</span></span>

- [<span data-ttu-id="123fd-136">User</span><span class="sxs-lookup"><span data-stu-id="123fd-136">User</span></span>](/graph/api/resources/user?view=graph-rest-1.0)
- <span data-ttu-id="123fd-137">[фотография](/graph/api/resources/profilephoto?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="123fd-137">[Photo](/graph/api/resources/profilephoto?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="123fd-138">[почта](/graph/api/resources/message?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="123fd-138">[Mail](/graph/api/resources/message?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="123fd-139">[календарь (пользователи и группы)](/graph/api/resources/event?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="123fd-139">[Calendar (users and groups)](/graph/api/resources/event?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="123fd-140">[контакт](/graph/api/resources/contact?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="123fd-140">[Contact](/graph/api/resources/contact?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="123fd-141">[вложение](/graph/api/resources/attachment?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="123fd-141">[Attachment](/graph/api/resources/attachment?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="123fd-142">[групповые чаты](/graph/api/resources/conversation?view=graph-rest-1.0);</span><span class="sxs-lookup"><span data-stu-id="123fd-142">[Group conversations](/graph/api/resources/conversation?view=graph-rest-1.0)</span></span>
- <span data-ttu-id="123fd-143">[люди и социальные медиа](/graph/api/resources/social-overview?view=graph-rest-beta);</span><span class="sxs-lookup"><span data-stu-id="123fd-143">[People and social](/graph/api/resources/social-overview?view=graph-rest-beta)</span></span>
- <span data-ttu-id="123fd-144">[хранилище (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="123fd-144">[Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)</span></span>
- [<span data-ttu-id="123fd-145">внешний элемент (Поиск Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="123fd-145">External item (Microsoft Search)</span></span>](/graph/api/resources/externalitem?view=graph-rest-beta)
- [<span data-ttu-id="123fd-146">Отчет</span><span class="sxs-lookup"><span data-stu-id="123fd-146">Report</span></span>](/graph/api/resources/report)
- [<span data-ttu-id="123fd-147">Подписка</span><span class="sxs-lookup"><span data-stu-id="123fd-147">Subscription</span></span>](/graph/api/resources/subscription)
- [<span data-ttu-id="123fd-148">Запрос на оценку угроз</span><span class="sxs-lookup"><span data-stu-id="123fd-148">Threat assessment request</span></span>](/graph/api/resources/threatassessmentrequest)
- [<span data-ttu-id="123fd-149">Запрос на оценку почты</span><span class="sxs-lookup"><span data-stu-id="123fd-149">Mail assessment request</span></span>](/graph/api/resources/mailassessmentrequest)
- [<span data-ttu-id="123fd-150">Запрос на оценку файла электронной почты</span><span class="sxs-lookup"><span data-stu-id="123fd-150">Email file assessment request</span></span>](/graph/api/resources/emailfileassessmentrequest)
- [<span data-ttu-id="123fd-151">Запрос на оценку файла</span><span class="sxs-lookup"><span data-stu-id="123fd-151">File assessment request</span></span>](/graph/api/resources/fileassessmentrequest)
- [<span data-ttu-id="123fd-152">Запрос на оценку URL-адреса</span><span class="sxs-lookup"><span data-stu-id="123fd-152">URL assessment request</span></span>](/graph/api/resources/urlassessmentrequest)
- [<span data-ttu-id="123fd-153">Результаты оценки угроз</span><span class="sxs-lookup"><span data-stu-id="123fd-153">Threat assessment result</span></span>](/graph/api/resources/threatassessmentresult)
- [<span data-ttu-id="123fd-154">Популярное</span><span class="sxs-lookup"><span data-stu-id="123fd-154">Trending</span></span>](/graph/api/resources/insights-trending)
- [<span data-ttu-id="123fd-155">Используемая аналитика</span><span class="sxs-lookup"><span data-stu-id="123fd-155">Used insight</span></span>](/graph/api/resources/insights-used)
- [<span data-ttu-id="123fd-156">Совместная аналитика</span><span class="sxs-lookup"><span data-stu-id="123fd-156">Shared insight</span></span>](/graph/api/resources/insights-shared)
- [<span data-ttu-id="123fd-157">Параметры пользователя</span><span class="sxs-lookup"><span data-stu-id="123fd-157">User settings</span></span>](/graph/api/resources/usersettings)
- [<span data-ttu-id="123fd-158">Приглашение</span><span class="sxs-lookup"><span data-stu-id="123fd-158">Invitation</span></span>](/graph/api/resources/invitation)

<span data-ttu-id="123fd-159">Развернутое описание регулирования в Microsoft Cloud см. в статье [Модель регулирования](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span><span class="sxs-lookup"><span data-stu-id="123fd-159">For a broader discussion of throttling in the Microsoft Cloud, see [Throttling pattern](https://docs.microsoft.com/azure/architecture/patterns/throttling).</span></span>

> [!NOTE]
> <span data-ttu-id="123fd-160">Если в ответе не предоставляется заголовок `Retry-After`, рекомендуем реализовать политику повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="123fd-160">If no `Retry-After` header is provided by the response, we recommend implementing an exponential backoff retry policy.</span></span> <span data-ttu-id="123fd-161">Вы также можете реализовать [более сложные шаблоны](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) при создании крупномасштабных приложений.</span><span class="sxs-lookup"><span data-stu-id="123fd-161">You can also implement [more advanced patterns](https://docs.microsoft.com/azure/architecture/patterns/category/resiliency) when building large-scale applications.</span></span>
>
> <span data-ttu-id="123fd-162">В пакетах SDK Microsoft Graph уже реализованы обработчики, основанные на заголовке `Retry-After` или (по умолчанию) на политике повторения экспоненциальной задержки.</span><span class="sxs-lookup"><span data-stu-id="123fd-162">Microsoft Graph SDKs already implement handlers that rely on the `Retry-After` header or default to an exponential backoff retry policy.</span></span>

## <a name="best-practices-to-avoid-throttling"></a><span data-ttu-id="123fd-163">Рекомендации по избежанию регулирования</span><span class="sxs-lookup"><span data-stu-id="123fd-163">Best practices to avoid throttling</span></span>

<span data-ttu-id="123fd-164">Шаблоны программирования, например постоянные опросы на ресурсе для проверки обновлений и регулярное сканирование коллекций ресурсов для проверки новых или удаленных ресурсов, чаще ведут к регулированию приложений и ухудшению общей производительности.</span><span class="sxs-lookup"><span data-stu-id="123fd-164">Programming patterns like continuously polling a resource to check for updates and regularly scanning resource collections to check for new or deleted resources are more likely to lead to applications being throttled and degrade overall performances.</span></span> <span data-ttu-id="123fd-165">Вместо этого необходимо по возможности использовать [отслеживание изменений](delta-query-overview.md) и [уведомления об изменениях](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="123fd-165">You should instead leverage [change tracking](delta-query-overview.md) and [change notifications](webhooks.md) when available.</span></span>

>[!NOTE]
><span data-ttu-id="123fd-166">Подробные сведения — в [рекомендациях по обнаружению файлов и определению изменений в масштабе](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).</span><span class="sxs-lookup"><span data-stu-id="123fd-166">[Best practices for discovering files and detecting changes at scale](https://docs.microsoft.com/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online) describes best practices in details.</span></span>

## <a name="service-specific-limits"></a><span data-ttu-id="123fd-167">Ограничения для отдельных служб</span><span class="sxs-lookup"><span data-stu-id="123fd-167">Service-specific limits</span></span>

<span data-ttu-id="123fd-168">Microsoft Graph позволяет получать доступ к данным в [нескольких службах](overview-major-services.md), таких как Outlook или Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="123fd-168">Microsoft Graph allows you to access data in [multiple services](overview-major-services.md), such as Outlook or Azure Active Directory.</span></span> <span data-ttu-id="123fd-169">В этих службах применяются собственные ограничения, которые влияют на работу приложений, использующих Microsoft Graph для доступа к ним.</span><span class="sxs-lookup"><span data-stu-id="123fd-169">These services impose their own throttling limits that affect applications that use Microsoft Graph to access them.</span></span>

> [!NOTE]
> <span data-ttu-id="123fd-170">Описанные здесь отдельные ограничения могут изменяться.</span><span class="sxs-lookup"><span data-stu-id="123fd-170">The specific limits described here are subject to change.</span></span>

> <span data-ttu-id="123fd-171">**Примечание.** В этом разделе термин *“клиент”* обозначает организацию Microsoft 365, в которой установлено приложение.</span><span class="sxs-lookup"><span data-stu-id="123fd-171">**Note:** In this section, the term *tenant* refers to the Microsoft 365 organization where the application is installed.</span></span> <span data-ttu-id="123fd-172">Этот клиент может быть тем же самым, что и клиент, с которым создавалось приложение, в случае приложения с одним клиентом, или же он может отличаться в случае с [приложением, включающим несколько клиентов](/azure/active-directory/develop/setup-multi-tenant-app).</span><span class="sxs-lookup"><span data-stu-id="123fd-172">This tenant can be the same as the the one where the application was created, in the case of a single tenant application, or it can be different, in the case of a [multi-tenant application](/azure/active-directory/develop/setup-multi-tenant-app).</span></span>

### <a name="outlook-service-limits"></a><span data-ttu-id="123fd-173">Ограничения службы Outlook</span><span class="sxs-lookup"><span data-stu-id="123fd-173">Outlook service limits</span></span>

<span data-ttu-id="123fd-174">Ограничения службы Outlook проверяются для каждого идентификатора приложения и сочетания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="123fd-174">Outlook service limits are evaluated for each app ID and mailbox combination.</span></span> <span data-ttu-id="123fd-175">Иными словами, описываемые ограничения применяются к конкретному приложению, которое получает доступ к определенному почтовому ящику (пользователя или группы).</span><span class="sxs-lookup"><span data-stu-id="123fd-175">In other words, the limits described apply to a specific app accessing a specific mailbox (user or group).</span></span> <span data-ttu-id="123fd-176">Если приложение превышает ограничение для одного почтового ящика, оно не повлияет на возможность доступа к другому почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="123fd-176">If an application exceeds the limit in one mailbox, it does not affect the ability to access another mailbox.</span></span> <span data-ttu-id="123fd-177">Указанные ниже ограничения относятся к общедоступному облаку, а также к [национальным облачным развертываниям](/graph/deployments).</span><span class="sxs-lookup"><span data-stu-id="123fd-177">The following limits apply to the public cloud as well as [national cloud deployments](/graph/deployments).</span></span>

| <span data-ttu-id="123fd-178">Ограничение</span><span class="sxs-lookup"><span data-stu-id="123fd-178">Limit</span></span>                                                      | <span data-ttu-id="123fd-179">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="123fd-179">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="123fd-180">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="123fd-180">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="123fd-181">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="123fd-181">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="123fd-182">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="123fd-182">4 concurrent requests</span></span>                                      | <span data-ttu-id="123fd-183">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="123fd-183">v1.0 and beta endpoints</span></span>   |
| <span data-ttu-id="123fd-184">Отправка 15 мегабайт (МБ) (PATCH, POST, PUT) в течение 30 секунд.</span><span class="sxs-lookup"><span data-stu-id="123fd-184">15 megabytes (MB) upload (PATCH, POST, PUT) in a 30 second period</span></span> | <span data-ttu-id="123fd-185">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="123fd-185">v1.0 and beta endpoints</span></span>   |

#### <a name="outlook-service-resources"></a><span data-ttu-id="123fd-186">Ресурсы службы Outlook</span><span class="sxs-lookup"><span data-stu-id="123fd-186">Outlook service resources</span></span>

<span data-ttu-id="123fd-187">Службой Outlook представляются нижеперечисленные ресурсы.</span><span class="sxs-lookup"><span data-stu-id="123fd-187">The following resources are provided by the Outlook service.</span></span>

##### <a name="calendar-api-resources"></a><span data-ttu-id="123fd-188">Ресурсы API календаря</span><span class="sxs-lookup"><span data-stu-id="123fd-188">Calendar API resources</span></span>

- [<span data-ttu-id="123fd-189">event</span><span class="sxs-lookup"><span data-stu-id="123fd-189">event</span></span>](/graph/api/resources/event)
- [<span data-ttu-id="123fd-190">eventMessage</span><span class="sxs-lookup"><span data-stu-id="123fd-190">eventMessage</span></span>](/graph/api/resources/eventmessage)
- [<span data-ttu-id="123fd-191">calendar</span><span class="sxs-lookup"><span data-stu-id="123fd-191">calendar</span></span>](/graph/api/resources/calendar)
- [<span data-ttu-id="123fd-192">calendarGroup</span><span class="sxs-lookup"><span data-stu-id="123fd-192">calendarGroup</span></span>](/graph/api/resources/calendargroup)
- [<span data-ttu-id="123fd-193">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="123fd-193">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="123fd-194">attachment</span><span class="sxs-lookup"><span data-stu-id="123fd-194">attachment</span></span>](/graph/api/resources/attachment)
- [<span data-ttu-id="123fd-195">place (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="123fd-195">place (preview)</span></span>](/graph/api/resources/place)

##### <a name="mail-api-resources"></a><span data-ttu-id="123fd-196">Ресурсы API почты</span><span class="sxs-lookup"><span data-stu-id="123fd-196">Mail API resources</span></span>

- [<span data-ttu-id="123fd-197">message</span><span class="sxs-lookup"><span data-stu-id="123fd-197">message</span></span>](/graph/api/resources/message)
- [<span data-ttu-id="123fd-198">mailFolder</span><span class="sxs-lookup"><span data-stu-id="123fd-198">mailFolder</span></span>](/graph/api/resources/mailfolder)
- [<span data-ttu-id="123fd-199">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="123fd-199">mailSearchFolder</span></span>](/graph/api/resources/mailsearchfolder)
- [<span data-ttu-id="123fd-200">messageRule</span><span class="sxs-lookup"><span data-stu-id="123fd-200">messageRule</span></span>](/graph/api/resources/messagerule)
- [<span data-ttu-id="123fd-201">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="123fd-201">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="123fd-202">attachment</span><span class="sxs-lookup"><span data-stu-id="123fd-202">attachment</span></span>](/graph/api/resources/attachment)

##### <a name="personal-contacts-api-resources"></a><span data-ttu-id="123fd-203">Ресурсы API для управления личными контактами</span><span class="sxs-lookup"><span data-stu-id="123fd-203">Personal contacts API resources</span></span>

- [<span data-ttu-id="123fd-204">contact</span><span class="sxs-lookup"><span data-stu-id="123fd-204">contact</span></span>](/graph/api/resources/contact)
- [<span data-ttu-id="123fd-205">contactFolder</span><span class="sxs-lookup"><span data-stu-id="123fd-205">contactFolder</span></span>](/graph/api/resources/contactfolder)
- [<span data-ttu-id="123fd-206">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="123fd-206">outlookCategory</span></span>](/graph/api/resources/outlookcategory)

##### <a name="social-and-workplace-intelligence-resources"></a><span data-ttu-id="123fd-207">Ресурсы социальной и рабочей аналитики</span><span class="sxs-lookup"><span data-stu-id="123fd-207">Social and workplace intelligence resources</span></span>

- [<span data-ttu-id="123fd-208">person</span><span class="sxs-lookup"><span data-stu-id="123fd-208">person</span></span>](/graph/api/resources/person)

##### <a name="to-do-tasks-api-preview-resources"></a><span data-ttu-id="123fd-209">Ресурсы API задач из списка дел (предварительный просмотр)</span><span class="sxs-lookup"><span data-stu-id="123fd-209">To-do tasks API (preview) resources</span></span>

- [<span data-ttu-id="123fd-210">outlookTask</span><span class="sxs-lookup"><span data-stu-id="123fd-210">outlookTask</span></span>](/graph/api/resources/outlooktask)
- [<span data-ttu-id="123fd-211">outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="123fd-211">outlookTaskFolder</span></span>](/graph/api/resources/outlooktaskfolder)
- [<span data-ttu-id="123fd-212">outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="123fd-212">outlookTaskGroup</span></span>](/graph/api/resources/outlooktaskgroup)
- [<span data-ttu-id="123fd-213">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="123fd-213">outlookCategory</span></span>](/graph/api/resources/outlookcategory)
- [<span data-ttu-id="123fd-214">attachment</span><span class="sxs-lookup"><span data-stu-id="123fd-214">attachment</span></span>](/graph/api/resources/attachment)

### <a name="cloud-communication-service-limits"></a><span data-ttu-id="123fd-215">Ограничения службы облачного взаимодействия</span><span class="sxs-lookup"><span data-stu-id="123fd-215">Cloud communication service limits</span></span>

| <span data-ttu-id="123fd-216">Ресурс</span><span class="sxs-lookup"><span data-stu-id="123fd-216">Resource</span></span>      | <span data-ttu-id="123fd-217">Ограничения на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="123fd-217">Limits per app per tenant</span></span>    |
| -------------- | ------------ |
| [<span data-ttu-id="123fd-218">Звонки</span><span class="sxs-lookup"><span data-stu-id="123fd-218">Calls</span></span>](/graph/api/resources/call) | <span data-ttu-id="123fd-219">10 000 звонков в месяц и 100 параллельных вызовов</span><span class="sxs-lookup"><span data-stu-id="123fd-219">10,000 calls/month and 100 concurrent calls</span></span>   |
| [<span data-ttu-id="123fd-220">Сведения о собрании</span><span class="sxs-lookup"><span data-stu-id="123fd-220">Meeting information</span></span>](/graph/api/resources/meetinginfo)   | <span data-ttu-id="123fd-221">2000 собраний на пользователя каждый месяц</span><span class="sxs-lookup"><span data-stu-id="123fd-221">2000 meetings/user each month</span></span> |
| <span data-ttu-id="123fd-222">[Присутствие](/graph/api/resources/presence) (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="123fd-222">[Presence](/graph/api/resources/presence) (preview)</span></span>   | <span data-ttu-id="123fd-223">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-223">2 rps</span></span> |

### <a name="project-rome-service-limits"></a><span data-ttu-id="123fd-224">Ограничения службы Project Rome</span><span class="sxs-lookup"><span data-stu-id="123fd-224">Project Rome service limits</span></span>

<span data-ttu-id="123fd-225">| Тип запроса | Ограничение на пользователя для всех приложений | | GET          | 400 запросов в течение 5 минут и 12000 запросов в течение 1 дня | | POST, PUT, PATCH, DELETE | 100 запросов в течение 5 минут и 8000 запросов в течение 1 дня |</span><span class="sxs-lookup"><span data-stu-id="123fd-225">| Request type | Limit per user for all apps | | GET          | 400 requests per 5 minutes and 12000 requests per 1 day | | POST, PUT, PATCH, DELETE | 100 requests per 5 minutes and 8000 requests per 1 day |</span></span>

<span data-ttu-id="123fd-226">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="123fd-226">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="123fd-227">activityHistoryItem, userActivity</span><span class="sxs-lookup"><span data-stu-id="123fd-227">activityHistoryItem, userActivity</span></span>

### <a name="microsoft-teams-service-limits"></a><span data-ttu-id="123fd-228">Ограничения службы Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="123fd-228">Microsoft Teams service limits</span></span>

<span data-ttu-id="123fd-229">Ограничения выражаются в виде запросов в секунду (RPS).</span><span class="sxs-lookup"><span data-stu-id="123fd-229">Limits are expressed as requests per second (rps).</span></span>

| <span data-ttu-id="123fd-230">Тип запроса Teams</span><span class="sxs-lookup"><span data-stu-id="123fd-230">Teams request type</span></span>                                   | <span data-ttu-id="123fd-231">Лимит на приложение на одного арендатора</span><span class="sxs-lookup"><span data-stu-id="123fd-231">Limit per app per tenant</span></span>        | <span data-ttu-id="123fd-232">Ограничение на приложение для всех арендаторов</span><span class="sxs-lookup"><span data-stu-id="123fd-232">Limit per app across all tenants</span></span>      |
|------------------------------------------------------|---------------------------------|------------|
| <span data-ttu-id="123fd-233">Любой API Graph призывает Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="123fd-233">Any Graph API calls for Microsoft Teams</span></span>              | <span data-ttu-id="123fd-234">15000 запросов каждые 10 секунд</span><span class="sxs-lookup"><span data-stu-id="123fd-234">15000 requests every 10 seconds</span></span> | <span data-ttu-id="123fd-235">н/д</span><span class="sxs-lookup"><span data-stu-id="123fd-235">n/a</span></span> |
| <span data-ttu-id="123fd-236">ПОЛУЧИТЬ команду, канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="123fd-236">GET team, channel, tab, installedApps, appCatalogs</span></span>   | <span data-ttu-id="123fd-237">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-237">60 rps</span></span>                          | <span data-ttu-id="123fd-238">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-238">600 rps</span></span> |
| <span data-ttu-id="123fd-239">Канал POST / PUT, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="123fd-239">POST/PUT channel, tab, installedApps, appCatalogs</span></span>    |  <span data-ttu-id="123fd-240">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-240">30 rps</span></span>                         | <span data-ttu-id="123fd-241">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-241">300 rps</span></span>  |
| <span data-ttu-id="123fd-242">PATCH команда, канал, вкладка, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="123fd-242">PATCH team, channel, tab, installedApps, appCatalogs</span></span> |  <span data-ttu-id="123fd-243">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-243">30 rps</span></span>                         | <span data-ttu-id="123fd-244">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-244">300 rps</span></span>  |
| <span data-ttu-id="123fd-245">УДАЛИТЬ канал, вкладку, установленные приложения, каталог приложений</span><span class="sxs-lookup"><span data-stu-id="123fd-245">DELETE channel, tab, installedApps, appCatalogs</span></span>      |  <span data-ttu-id="123fd-246">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-246">15 rps</span></span>                         | <span data-ttu-id="123fd-247">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-247">150 rps</span></span>  |
| <span data-ttu-id="123fd-248">Получить /teams/```{team-id}```, joinedTeams</span><span class="sxs-lookup"><span data-stu-id="123fd-248">GET /teams/```{team-id}```, joinedTeams</span></span>              |  <span data-ttu-id="123fd-249">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-249">30 rps</span></span>                         | <span data-ttu-id="123fd-250">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-250">300 rps</span></span>  |
| <span data-ttu-id="123fd-251">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, клон</span><span class="sxs-lookup"><span data-stu-id="123fd-251">POST /teams/```{team-id}```, PUT /groups/```{team-id}```/team, clone</span></span> | <span data-ttu-id="123fd-252">6 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-252">6 rps</span></span> | <span data-ttu-id="123fd-253">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-253">150 rps</span></span>  | 
| <span data-ttu-id="123fd-254">ПОЛУЧИТЬ сообщение канала</span><span class="sxs-lookup"><span data-stu-id="123fd-254">GET channel message</span></span>  | <span data-ttu-id="123fd-255">5 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-255">5 rps</span></span> | <span data-ttu-id="123fd-256">100 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-256">100 rps</span></span> |
| <span data-ttu-id="123fd-257">ПОЛУЧИТЬ 1: 1 / сообщение группового чата</span><span class="sxs-lookup"><span data-stu-id="123fd-257">GET 1:1/group chat message</span></span>  | <span data-ttu-id="123fd-258">3 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-258">3 rps</span></span> | <span data-ttu-id="123fd-259">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-259">30 rps</span></span> |
| <span data-ttu-id="123fd-260">Сообщение POST канала</span><span class="sxs-lookup"><span data-stu-id="123fd-260">POST channel message</span></span> | <span data-ttu-id="123fd-261">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-261">2 rps</span></span> | <span data-ttu-id="123fd-262">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-262">20 rps</span></span> |
| <span data-ttu-id="123fd-263">POST 1: 1 / сообщение в групповом чате</span><span class="sxs-lookup"><span data-stu-id="123fd-263">POST 1:1/group chat message</span></span> | <span data-ttu-id="123fd-264">2 запроса в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-264">2 rps</span></span> | <span data-ttu-id="123fd-265">20 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-265">20 rps</span></span> |
| <span data-ttu-id="123fd-266">GET /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="123fd-266">GET /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="123fd-267">60 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-267">60 rps</span></span> | <span data-ttu-id="123fd-268">600 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-268">600 rps</span></span> |
| <span data-ttu-id="123fd-269">POST, PATCH, PUT /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="123fd-269">POST, PATCH, PUT /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="123fd-270">30 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-270">30 rps</span></span> | <span data-ttu-id="123fd-271">300 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-271">300 rps</span></span> |
| <span data-ttu-id="123fd-272">DELETE /teams/```{team-id}```/schedule и все API по этому пути</span><span class="sxs-lookup"><span data-stu-id="123fd-272">DELETE /teams/```{team-id}```/schedule and all APIs under this path</span></span> | <span data-ttu-id="123fd-273">15 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-273">15 rps</span></span> | <span data-ttu-id="123fd-274">150 запросов в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-274">150 rps</span></span> |

<span data-ttu-id="123fd-275">Максимально 4 запроса в секунду на приложение могут быть отправлены для данной команды или канала.</span><span class="sxs-lookup"><span data-stu-id="123fd-275">A maximum of 4 requests per second per app can be issued on a given team or channel.</span></span>
<span data-ttu-id="123fd-276">Приложение может отправлять в определенный канал не более 3000 сообщений в день.</span><span class="sxs-lookup"><span data-stu-id="123fd-276">A maximum of 3000 messages per app per day can be sent to a given channel.</span></span>

<span data-ttu-id="123fd-277">См. Также [ограничения Microsoft Teams](/graph/api/resources/teams-api-overview#microsoft-teams-limits) и [требования к опросу](/graph/api/resources/teams-api-overview#polling-requirements).</span><span class="sxs-lookup"><span data-stu-id="123fd-277">See also [Microsoft Teams limits](/graph/api/resources/teams-api-overview#microsoft-teams-limits) and [polling requirements](/graph/api/resources/teams-api-overview#polling-requirements).</span></span>

### <a name="information-protection"></a><span data-ttu-id="123fd-278">Защита информации</span><span class="sxs-lookup"><span data-stu-id="123fd-278">Information protection</span></span>

<span data-ttu-id="123fd-279">Указанные ниже ограничения применяются к любому запросу в `/informationProtection`.</span><span class="sxs-lookup"><span data-stu-id="123fd-279">The following limits apply to any request on `/informationProtection`.</span></span>

| <span data-ttu-id="123fd-280">Операция</span><span class="sxs-lookup"><span data-stu-id="123fd-280">Operation</span></span>                 | <span data-ttu-id="123fd-281">Ограничение для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="123fd-281">Limit per tenant</span></span>                                            | <span data-ttu-id="123fd-282">Ограничение на ресурс (электронная почта, URL-адрес, файл)</span><span class="sxs-lookup"><span data-stu-id="123fd-282">Limit per resource (email, URL, file)</span></span>                |
|---------------------------|-------------------------------------------------------------|------------------------------------------------------|
| <span data-ttu-id="123fd-283">POST</span><span class="sxs-lookup"><span data-stu-id="123fd-283">POST</span></span>                      | <span data-ttu-id="123fd-284">150 запросов в течение 15 минут и 10000 запросов в течение 24 часов</span><span class="sxs-lookup"><span data-stu-id="123fd-284">150 requests per 15 minutes and 10000 requests per 24 hours</span></span> | <span data-ttu-id="123fd-285">1 запрос в течение 15 минут и 3 запроса в течение 24 часов</span><span class="sxs-lookup"><span data-stu-id="123fd-285">1 request per 15 minutes and 3 requests per 24 hours</span></span> |

<span data-ttu-id="123fd-286">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="123fd-286">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="123fd-287">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span><span class="sxs-lookup"><span data-stu-id="123fd-287">threatAssessmentRequest, threatAssessmentResult, mailAssessmentRequest, emailFileAssessmentRequest, fileAssessmentRequest, urlAssessmentRequest.</span></span>

### <a name="identity-protection-and-conditional-access-service-limits"></a><span data-ttu-id="123fd-288">Ограничения в отношении защиты удостоверений и службы условного доступа</span><span class="sxs-lookup"><span data-stu-id="123fd-288">Identity protection and conditional access service limits</span></span>

| <span data-ttu-id="123fd-289">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="123fd-289">Request type</span></span> | <span data-ttu-id="123fd-290">Ограничение для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="123fd-290">Limit per tenant</span></span> |
| ------------ | ------- |
| <span data-ttu-id="123fd-291">Любой</span><span class="sxs-lookup"><span data-stu-id="123fd-291">Any</span></span> | <span data-ttu-id="123fd-292">1 запрос в секунду</span><span class="sxs-lookup"><span data-stu-id="123fd-292">1 request per second</span></span> |

<span data-ttu-id="123fd-293">Указанные выше ограничения действуют для следующих ресурсов:</span><span class="sxs-lookup"><span data-stu-id="123fd-293">The preceding limits apply to the following resources:</span></span>  
<span data-ttu-id="123fd-294">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span><span class="sxs-lookup"><span data-stu-id="123fd-294">riskDetection, riskyUser, riskyUserHistoryItem, namedLocation, countryNamedLocation, ipNamedLocation, conditionalAccessPolicy.</span></span>

> <span data-ttu-id="123fd-295">**Примечание.** В настоящее время перечисленные выше ресурсы не возвращают заголовок `Retry-After` в ответах `429 Too Many Requests`.</span><span class="sxs-lookup"><span data-stu-id="123fd-295">**Note:** at the moment the resources listed above do not return a `Retry-After` header on `429 Too Many Requests` responses.</span></span>

### <a name="insights-service-limits"></a><span data-ttu-id="123fd-296">Ограничения службы аналитики</span><span class="sxs-lookup"><span data-stu-id="123fd-296">Insights service limits</span></span>

<span data-ttu-id="123fd-297">Указанные ниже ограничения применяются к любому запросу в `me/insights` или `users/{id}/insights`.</span><span class="sxs-lookup"><span data-stu-id="123fd-297">The following limits apply to any request on `me/insights` or `users/{id}/insights`.</span></span>

| <span data-ttu-id="123fd-298">Ограничение</span><span class="sxs-lookup"><span data-stu-id="123fd-298">Limit</span></span>                                                      | <span data-ttu-id="123fd-299">Сфера применения</span><span class="sxs-lookup"><span data-stu-id="123fd-299">Applies to</span></span>      |
|------------------------------------------------------------|-----------------|
| <span data-ttu-id="123fd-300">10 000 запросов API в течение 10-минутного периода</span><span class="sxs-lookup"><span data-stu-id="123fd-300">10,000 API requests in a 10 minute period</span></span>                  | <span data-ttu-id="123fd-301">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="123fd-301">v1.0 and beta endpoints</span></span> |
| <span data-ttu-id="123fd-302">4 параллельных запроса</span><span class="sxs-lookup"><span data-stu-id="123fd-302">4 concurrent requests</span></span>                                      | <span data-ttu-id="123fd-303">Конечные точки версии 1.0 и бета-версии</span><span class="sxs-lookup"><span data-stu-id="123fd-303">v1.0 and beta endpoints</span></span>   |

### <a name="microsoft-graph-reports-service-limits"></a><span data-ttu-id="123fd-304">Ограничения службы отчетов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="123fd-304">Microsoft Graph reports service limits</span></span>

<span data-ttu-id="123fd-305">Указанные ниже ограничения применяются к любому запросу в `/reports`.</span><span class="sxs-lookup"><span data-stu-id="123fd-305">The following limits apply to any request on `/reports`.</span></span>

| <span data-ttu-id="123fd-306">Операция</span><span class="sxs-lookup"><span data-stu-id="123fd-306">Operation</span></span>                 | <span data-ttu-id="123fd-307">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="123fd-307">Limit per app per tenant</span></span>     | <span data-ttu-id="123fd-308">Ограничение для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="123fd-308">Limit per tenant</span></span>           |
|---------------------------|------------------------------|----------------------------|
| <span data-ttu-id="123fd-309">Любой запрос (CSV)</span><span class="sxs-lookup"><span data-stu-id="123fd-309">Any request (CSV)</span></span>         | <span data-ttu-id="123fd-310">14 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="123fd-310">14 requests per 10 minutes</span></span>   | <span data-ttu-id="123fd-311">40 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="123fd-311">40 requests per 10 minutes</span></span> |
| <span data-ttu-id="123fd-312">Любой запрос (JSON, beta)</span><span class="sxs-lookup"><span data-stu-id="123fd-312">Any request (JSON, beta)</span></span>  | <span data-ttu-id="123fd-313">100 запросов в течение 10 минут</span><span class="sxs-lookup"><span data-stu-id="123fd-313">100 requests per 10 minutes</span></span>  | <span data-ttu-id="123fd-314">н/д</span><span class="sxs-lookup"><span data-stu-id="123fd-314">n/a</span></span>                        |

<span data-ttu-id="123fd-315">Указанные выше ограничения применяются по отдельности к каждому API отчетов.</span><span class="sxs-lookup"><span data-stu-id="123fd-315">The preceding limits apply individually to each report API.</span></span> <span data-ttu-id="123fd-316">Например, запрос на API отчетов об активности пользователей Microsoft Teams и запрос на доступ к отчету об активности пользователей Outlook в течение 10 минут будут рассматриваться как 1 запрос из 14 для каждого API, а не 2 запроса из 14 для обоих.</span><span class="sxs-lookup"><span data-stu-id="123fd-316">For example a request to Microsoft Teams user activity report API and a request to Outlook user activity report API within 10 minutes will count as 1 request out of 14 for each API, not 2 requests out of 14 for both.</span></span>

### <a name="invitation-manager-service-limits"></a><span data-ttu-id="123fd-317">Ограничения службы диспетчера приглашений</span><span class="sxs-lookup"><span data-stu-id="123fd-317">Invitation manager service limits</span></span>

<span data-ttu-id="123fd-318">Указанные ниже ограничения применяются к любому запросу в `/invitations`.</span><span class="sxs-lookup"><span data-stu-id="123fd-318">The following limits apply to any request on `/invitations`.</span></span>

| <span data-ttu-id="123fd-319">Операция</span><span class="sxs-lookup"><span data-stu-id="123fd-319">Operation</span></span>                 | <span data-ttu-id="123fd-320">Ограничение для каждого клиента</span><span class="sxs-lookup"><span data-stu-id="123fd-320">Limit per tenant</span></span>             |
|---------------------------|------------------------------|
| <span data-ttu-id="123fd-321">Любая операция</span><span class="sxs-lookup"><span data-stu-id="123fd-321">Any operation</span></span>             | <span data-ttu-id="123fd-322">150 запросов за 5 секунд</span><span class="sxs-lookup"><span data-stu-id="123fd-322">150 requests per 5 seconds</span></span>   |

### <a name="open-and-schema-extensions-service-limits"></a><span data-ttu-id="123fd-323">Ограничения службы для открытых расширений и расширений схемы</span><span class="sxs-lookup"><span data-stu-id="123fd-323">Open and schema extensions service limits</span></span>

| <span data-ttu-id="123fd-324">Тип запроса</span><span class="sxs-lookup"><span data-stu-id="123fd-324">Request type</span></span> | <span data-ttu-id="123fd-325">Ограничение на приложение по клиенту</span><span class="sxs-lookup"><span data-stu-id="123fd-325">Limit per app per tenant</span></span> |
| ------------ | ------------------------ |
| <span data-ttu-id="123fd-326">Любой</span><span class="sxs-lookup"><span data-stu-id="123fd-326">Any</span></span>          | <span data-ttu-id="123fd-327">455 запросов в течение 10 секунд</span><span class="sxs-lookup"><span data-stu-id="123fd-327">455 requests per 10 seconds</span></span> |

<span data-ttu-id="123fd-328">Указанные выше ограничения действуют для следующих ресурсов: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post и user.</span><span class="sxs-lookup"><span data-stu-id="123fd-328">The preceding limits apply to the following resources: openTypeExtension, schemaExtension, administrativeUnit, contact, device, event, group, message, organization, post, and user.</span></span>

<!-- { "blockType": "throttlinggenstart" } -->
### <a name="education-service-limits"></a><span data-ttu-id="123fd-329">Ограничения службы для образования</span><span class="sxs-lookup"><span data-stu-id="123fd-329">Education service limits</span></span>

[!INCLUDE [Education rostering APIS throttling documentation](../includes/throttling-education-rostering-apis.md)]

### <a name="excel-service-limits"></a><span data-ttu-id="123fd-330">Ограничения службы Excel</span><span class="sxs-lookup"><span data-stu-id="123fd-330">Excel service limits</span></span>

[!INCLUDE [Excel throttling documentation](../includes/throttling-excel.md)]

### <a name="identity-and-access-audit-logs-service-limits"></a><span data-ttu-id="123fd-331">Ограничения службы журналов аудита удостоверения и доступа</span><span class="sxs-lookup"><span data-stu-id="123fd-331">Identity and access audit logs service limits</span></span>

[!INCLUDE [Identity and access audit logs throttling documentation](../includes/throttling-Identity-and-access-audit-logs.md)]

### <a name="identity-providers-service-limits"></a><span data-ttu-id="123fd-332">Ограничения службы поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="123fd-332">Identity providers service limits</span></span>

[!INCLUDE [CPIM throttling documentation](../includes/throttling-cpim.md)]

### <a name="intune-service-limits"></a><span data-ttu-id="123fd-333">Ограничения службы Intune</span><span class="sxs-lookup"><span data-stu-id="123fd-333">Intune service limits</span></span>

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

### <a name="skype-service-limits"></a><span data-ttu-id="123fd-334">Ограничения службы Skype</span><span class="sxs-lookup"><span data-stu-id="123fd-334">Skype service limits</span></span>

[!INCLUDE [Skype calling throttling documentation](../includes/throttling-skype-calling.md)]

### <a name="subscription-service-limits"></a><span data-ttu-id="123fd-335">Ограничения службы подписки</span><span class="sxs-lookup"><span data-stu-id="123fd-335">Subscription service limits</span></span>

[!INCLUDE [Subscription services throttling documentation](../includes/throttling-subscription-services.md)]

<!-- { "blockType": "throttlinggenend" } -->
